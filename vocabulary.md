# Vocabulary
Having a shared vocabulary is important. It is even more important to understand the specific/company nuances around that vocabulary. Below are some terms that you may already know. But please take the time to read how we implement them.

## CI/CD
**Continuous Integration and Continuous Delivery**
Continuous integration is a process that kicks off every time a branch is pushed to GitHub/merged to master. CircleCI (our CI provider) will stand up a fresh Linux box, clone the branch, install the dependencies, and run the specs. If the specs don't pass, the branch/PR isn't merged.

Continuous Delivery is a process that follows CI. After CI passes, certain branches will be automatically deployed to their respective servers. Right now, the master branch will be deployed to the staging servers (and staging branches). From there, we will PR the staging branch to the production branch. IF that PR passing CI/CD, it will be deployed to production.

## MVC
**Model View Controller** A software architecture pattern that splits the concerns of the application into three different class types: Model - the central component and usually represented by a table in a database. View - the representation of information to the user (web pages, tables, charts, etc.)Controller - the translation layer between the other two types of classes, for instance, accepting input from a View to pass to a Model or formatting data from Model to pass to a View.

## MVP
**Minimally Viable Product** This is a slightly more tuned version of a POC. Unlike a POC, an MVP contains tested, well thought out code. It is built with pride. It is built with the idea that it will slowly, but surely turn into a full-featured application. But like a POC, this application is considered 'done' once it has barely enough features to work. An MVP may have authentication, authorization, and serve core needs. But it will NOT have 'all the bells and whistles'. Those bells/whistles will be bolted on as additional features as time goes on.

## POC
**Proof of Concept** A simple, quick way to build an application. The code behind this application may not be perfect, clean, or even tested. The goal of a POC is to get something that functions. It will almost assuredly have bugs. But if we can put in front of stakeholders and start a discussion around it, it is done. Having a POC shelved is common.

## TDD
**Test Driven Development**
You should already know this one. Testing code is important. But it is important to note are not dogmatic about when that code is tested. Write your tests before, during, or after building a feature. We really don't care. Just make sure it is fully tested before it is PR'ed. Also - if you are doing a bug fix, look for opportunities to write regression tests from keeping that bug from re-spawning in the future.

## UAT 
**User Acceptance Testing** A form of testing where an application or feature is released to a staging server and stakeholders are expected to test/report bugs. UAT passes when all features are working without any reported bugs. UAT is NOT the place/time to request/add additional features.
