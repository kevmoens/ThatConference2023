# Get Your Marshmallows Ready: Fun and Efficient Testing with Specflow

## Tuesday, July 25, 2023 - 4:00 PM CDT, for 1 hour

### AT THAT (In-Person Only) Regular, 60 minute presentation

### Room: C

Are you tired of boring and flavorless test automation? Then join us for a Specflow camping trip where we'll show you how to make your test automation journey fun and tasty!

In this session, we'll explore the benefits of using Specflow for test automation and share some tips and tricks for overcoming common challenges. Make your test data look like s'mores ingredients! And who knows? We might even find a way to work gherkins into our testing scenarios. After all, just like the gherkin syntax in Specflow, a little bit of this zesty pickle can add a lot of flavor and spice to any dish - or any code!

We'll also share some best practices for organizing and maintaining your Specflow tests, including how to create reusable step definitions and how to manage test data efficiently.

So pack your virtual camping gear and join us for a fun and tasty journey through test automation with Specflow as your guide. We promise it'll be a trip to remember!

## SpecFlow Install

- In Visual Studio Open
  - Extensions
    - Manage Extensions
      - Online - Search - Specflow
      - Install Specflow for Visual Studio "version"

## LivingDoc Install

- Add NuGet package SpecFlow.Plus.LivingDocPlugin
- dotnet tool install --global SpecFlow.Plus.LivingDoc.CLI
- livingdoc test-assembly RequestTimeOff.Specflow.dll -t TestExecution.json
  - Execute inside of .\Project.Specflow\bin\Debug\net7.0
