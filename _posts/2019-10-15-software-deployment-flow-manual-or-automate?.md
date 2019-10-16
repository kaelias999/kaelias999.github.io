---
layout: post
title:  "Software deployment, Manual or Automate?"
date:   2019-10-15 00:16:00 +0700
categories: [devops]
---

Software deployment has always been a core part of Software life cycle and there has always been debate between doing it manually or automation.
Personally, i think the advantage of Automate Deployment (or we can call `Deployment PipeLine`) is quite obvious but the preparation and the amount of work needed to adapt such method is what has kept most people from it.

Here is some pros and cons that i can think of right now about each deployment method:

1. Manual Deployment
    - Pros:
        - Easy to do.
        - No need to use third party software.
    - Cons:
        - Deployment method doesn't follow any standard guideline but instead depend heavily on personal approach.
        - Very hard to control the state of each server after deployment : config, version, library etc.
        - Hard to transfer knowledge between people.
        - Deployment might take long time to prepare and is error prone cause the testing environment might be different from production environment
        - Hard to roll back.
2. Deployment Pipeline
    - Pros:
        - Using Standard flow which has been widely accepted in the world.
        - Easy to control state of each server since everything can be stored as code on Git or version control software.
        - Easy to transfer knowledge.
        - Roll back is easy and fast.
        - Deployment process is fast and less prone to error.
    - Cons:
        - Take long time and investment to adapt and build the pipeline.
        - Stricter working process for both developers and sys admin.


For all of the above, it's quite clear that the winner in the long-run will be to adapt Deployment PipeLine in your deployment process. The Pros should worth the initial investment of time and human resource that you have to spend.

For the next post i will talk about how to build a simple deployment pipeline.