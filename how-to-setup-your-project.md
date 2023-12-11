# How to Setup your Open Source Project

There are a lot of things to consider when setting up your open source project. In this portion of the guide, we will walk through key components that every project needs to be successful.

## How to Write an Installation Guide for Contributors

When a new contributor is interested in working with your project, they will need a clear step by step guide on how to setup everything locally. This guide should include the following items:

- instructions for forking the repository
- instructions for cloning the repository
- instructions for installing the dependencies 
- instructions for setting up the environment variables
- instructions for setting up the database if applicable 
- instructions for running the project locally
- instructions for setting up Docker containers if applicable

The best way to test your guide is by setting up the project locally using your guide. You will learn quickly if anything is missing or not clear if you run into issues getting your project to work. 

### Where to Place the Installation Guide

The best place for installation instructions should be in your project's `README.md` file. This will be the most accessible file for your contributors. It would good to have a section at the top for setting up the project locally. 

Another good place would be in the `CONTRIBUTING.md` file. This file is used to cover topics like installation setup, testing, linting, workflows, etc. You can place the installation instruction towards the top of your  `CONTRIBUTING.md` file. 

If your project is on the larger side, then you might consider having a separate documentation site and dedicating a section for installation in there. You can use documentation site generators like [docsify](https://docsify.js.org/#/), [Docusaurus](https://docusaurus.io/) or [Starlight](https://starlight.astro.build/).

## How to Choose a License for Your Project

## How to Write a Code Of Conduct

## How create Contributing Guides

## How to Write a Good README

## How to Create Issue Templates

## How to Creating PR Templates

## How to Work with GitHub Project Boards
