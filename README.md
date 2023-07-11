# Abstract App Building Workshop

This workshop will be a hands-on introduction to building apps with [Abstract](https://abstract.money). We'll be completing a dollar-cost-averaging app that will allow users to set up recurring purchases of a token of their choice. The goal of the workshop is to have the app's tests passing by the end of the workshop, setting you up to build your own apps with Abstract.

## Prerequisites

Have a brief look at the required prerequisites [here](https://docs.abstract.money/4_get_started/2_installation.html). The recommended tools won't be required for this workshop.

> You can run `cargo check` to make sure that the application compiles.
> You can then run `cargo test` to see the failing tests.

## Outline

A high-level introduction to Abstract will be given, followed by the use-case of the application and a brief overview of the codebase. We'll then dive into the code and complete the app together in Quests.

## Application

The application we're building is a dollar-cost-averaging application that allows the owner of an Abstract smart-contract wallet to set up recurring purchases of a token of their choice. The user will be able to set the amount of tokens they want to purchase, the frequency of the purchases, and the token they want to purchase. The application will then automatically purchase the tokens for the user at the specified frequency.

## Codebase

The working codebase can be found in [our monorepo](https://github.com/AbstractSDK/abstract/tree/main/modules/contracts/apps/dca).

## Quests

The quests consist of a series of missing code snippets that you'll need to complete in order to get the application to work. The quests are numbered by `#{quest_number}`. At the beginning of each quest you can search for that and find the locations that need fixing.

## Quest 0: Module Dependencies

Module dependencies define what other modules the application requires to perform its logic. This segregation of concerns allows for more modular applications that can be reused in different contexts.

> To find the code that needs work, search for `#0` in your IDE of choice.

## Quest 1: Admin Validation

Each application has an `admin` that is able to perform administrative actions on the application. In this case, the `admin` is the owner of the Abstract smart-contract wallet that the application is installed on. We need to make sure that the `admin` is the one calling the administrative functions.

> To find the code that needs work, search for `#1` in your IDE of choice.

## Quest 2: Abstract SDK composable APIs

The [`abstract-sdk`]() allows developers to create APIs for their modules. These APIs allow users of that module to interact with it in an intuitive way. In this quest we'll be using the Dex and CronCat APIs to perform token swaps and schedule recurring transactions.
