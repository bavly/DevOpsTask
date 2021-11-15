# devops-techtask

## Overview

Hopefully this tech task allows you to strut your stuff as much as you decide to!

This exercise should take you no more than a weekend. If you need any clarification, please don’t hesitate to ask us.

## Task details

This repository contains a simple golang service which serves a single endpoint: `/:id`. For each call to this endpoint, the service increments a counter, and returns the number of times the endpoint has been called for the given ID. State for the application is stored in and retrieved from redis, where the data is stored simply with `id` as the key, and the count as the value.

We'd like to deploy this application, and all its dependencies (in this case, redis) on kubernetes. It should be accessible from outside the cluster via HTTP, and should be deployed with high-availability in mind. You are highly encouraged to use any infrastructure automation or deployment tools that you are familiar with to do this. 

The entire solution should be able to run on an fresh ubuntu VM.

You may modify the application code as you see fit, but ensure that the functionality remains the same.

In your solution, include a readme containing the necessary steps to set up the environment, as well as to build, package and deploy the application. Also detail and explain your chosen architecture, as well as what tools were used in the deployment process.

## Requirements

- Simple to build and run
- Application is able to be deployed on kubernetes and can be accessed from outside the cluster
- Application must be able to survive the failure of one or more instances while staying highly-available
- Redis must be password protected
- Readme documents how to run the code and provides explanation regarding the implementation

