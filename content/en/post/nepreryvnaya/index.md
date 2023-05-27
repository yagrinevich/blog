---
title: Continuous Integration and Continuous Deployment (CI/CD)
subtitle: Learn the difference between these continuous methods
summary: What is the difference between continuous integration, continuous delivery, and continuous deployment (CI/CD)?
authors:
  - admin
tags: []
categories: []
projects: []
date: '2019-02-05T00:00:00Z'
lastMod: '2019-09-05T00:00:00Z'
image:
  caption: ''
  focal_point: ''
---


## Continuous Integration

Developers who use continuous integration merge their changes back into the main branch whenever possible. Changes made by a developer are verified by creating an assembly and running automated tests on that assembly. With this approach, you avoid the hassle of integrating when you have to wait for release day to merge changes in the relevant branch.

When using continuous integration, a lot of attention is paid to test automation, as a result of which, when integrating new commits into the main branch, the application does not break.

## Continuous supply

Continuous delivery is an extension of continuous integration because it automatically deploys all code changes to the test and/or production environment after the build step.

This means that not only the testing process is automated, but also the product release process, so the application can be deployed at any time with one click.

Theoretically, with continuous delivery, you can release daily, weekly, every two weeks, or any other business-relevant frequency. However, if you really want to take advantage of continuous delivery, you should deploy to production as early as possible, ensuring that small patches are released that are easy to find bugs in case of problems.
## Continuous deployment

Continuous Deployment goes one step further than Continuous Delivery. With this approach, every change that goes through all stages of the production pipeline is released to customers. No human intervention is required, and only an error during a test can prevent a new change from being deployed to production.

Continuous Deployment is a great way to speed up the customer feedback cycle and take the pressure off your team by canceling the “release day”. Developers can focus on creating software. They see how their code is launched in minutes, as soon as it is finished.

## How do these approaches relate to each other
Simply put, continuous integration is part of both continuous delivery and continuous deployment. And continuous deployment is similar to continuous delivery, except that releases happen automatically.
Continuous Deployment

This post was created with Jupyter. The orginal files can be found at https://github.com/gcushen/hugo-academic/tree/master/exampleSite/content/post/jupyter
