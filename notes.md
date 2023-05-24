# Get Your Marshmallows Ready: Fun and Efficient Testing with Specflow

## Tuesday, July 25, 2023 - 4:00 PM CDT, for 1 hour

### AT THAT (In-Person Only) Regular, 60 minute presentation

### Room: C

Are you tired of boring and flavorless test automation? Then join us for a Specflow camping trip where we'll show you how to make your test automation journey fun and tasty!

In this session, we'll explore the benefits of using Specflow for test automation and share some tips and tricks for overcoming common challenges. Make your test data look like s'mores ingredients! And who knows? We might even find a way to work gherkins into our testing scenarios. After all, just like the gherkin syntax in Specflow, a little bit of this zesty pickle can add a lot of flavor and spice to any dish - or any code!

We'll also share some best practices for organizing and maintaining your Specflow tests, including how to create reusable step definitions and how to manage test data efficiently.

So pack your virtual camping gear and join us for a fun and tasty journey through test automation with Specflow as your guide. We promise it'll be a trip to remember!

## Links 

[Wiki](https://en.wikipedia.org/wiki/Behavior-driven_development)

## TODO 
  
  Review Nich Chapsas Unit Testing from zero to hero.
  - Naming of unit test method 
  Specflow Examples, Tags

## Collaboration with your team

3 Amigos
Dave Farley - Continous Delivery YouTube Channel
  Dan North
  Liz Keogh
  Gojko Adzic
Goal - Better Software Faster
Software Development is a team sport
World Class Habits
  Avoid bureaucracy of very detailed specifications and needing a review by a senior developer, just work on making everyone more trustable.  This happens with World Class Habits

## User Stories

### What are user stories?

User stories are short, simple descriptions of a solution that your team has come up with, told from the perspective of the person who is playing out the interaction. They are part of a larger epic that describes the actual problem to be solved and why you’re solving it.

The operative word here is user, meaning a user story puts the focus on the user, not the product.

A user story usually focuses on three areas:

- As a (who)
- I want to (what)
- So that (why)

This is all usually followed by acceptance criteria, which define how you know if the interaction is successful.

## Acceptance Criteria

### Enter Gherkin

- Given
- When
- Then

Gherkins are a way to add to user stories and give a full scenario that will help developers and testers understand both the outcome and the output of a particular user interaction.

- Background - Shared Given portion of a feature
- Scenario — the behavior you’re going to describe
- Given — the beginning state of the scenario
- When — a specific action that the user takes
- Then — a testable outcome, usually caused by the action in When
- And — this continues any of the other three operations if necessary

Taking the password scenario previously described:

#### Example
Scenario: When setting a password,
- Given that I am an account admin,
- When I enter a password in the password field,
- Then I should be warned of the password requirements,
- And I should be allowed to make corrections right away,
- Then that I can create a secure account.

We now have a full picture of who is carrying out the specific action, and what the requirements are for the acceptance criteria, and the team knows what potential frustrations there might be so that they can ensure that the process flows more smoothly.

Generally, the product manager or product owner is responsible for writing out the Gherkin stories, thus creating better communication between the rest of the team and making sure that everyone is focusing on outcomes, not just outputs.

### Watch out for:

It always feel great to have every detail / question answered.  Caution in going overboard.  If you separate the thinking from doing you are loosing the value of different view points.  

## SpecFlow Install

- In Visual Studio Open
  - Extensions
    - Manage Extensions
      - Online - Search - Specflow
      - Install Specflow for Visual Studio "version"

## Parts of Specflow

  - Feature
  - Background
  - Scenario
  - Parameters
  - Examples (Outline)
  - Tables
  - Tags

## LivingDoc Install

- Add NuGet package SpecFlow.Plus.LivingDocPlugin
- dotnet tool install --global SpecFlow.Plus.LivingDoc.CLI
- livingdoc test-assembly RequestTimeOff.Specflow.dll -t TestExecution.json
  - Execute inside of .\Project.Specflow\bin\Debug\net7.0

## Continous Delivery vs Test Coverage

Imagine these two different examples.
It is 1980s and you are about to deliver Super Mario Bros for Nintendo Entertainment System.  
Compare that to today with apps like Netflix.  

Imagine finding an issue that stops the app from continuing.

What is the biggest difference?  

The NES game system doesn't connect to the internet.  You need to deliver the game / app with as little issues as possible.  In this case writing tests for as much as you can would be very important.  Any issue might result in your game not selling.

Netflix is known to regularly push 10 updates per week through their CI/CD pipeline.

The Super Mario Bros example might be an extreme example, but it isn't far off from some software that is still used today.  The company I work for sells ERP software and over 90% of clients are modified and over 80% are hosted on premise of the client.  With this scenario there isn't a simple method to get all clients up to date and run Continous Delivery.  
(Create Image with spectrum showing number of tests)

Note the more tests you have you can affect future development speed.

### Limiting Tests

https://youtu.be/Xc5gAyzQRzI