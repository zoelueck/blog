+++
title = 'Go Bot the First'
date = 2025-02-21T21:14:45+01:00
summary = "The first post in my journal of Discord Bot development, mainly design focused, not much coding yet"
+++

# Designing a discord bot
the idea behind this bot stems from a discord webhook pythonscript cron job ~~clusterfuck~~ setup i used to run in an old friend group to remind a couple people of things like taking medicine or doing other tasks, this was cumbersome and slow to do and as such i decided to tackle the issue with a proper bot, using modern technology from go to argo or flux cd

## Initial ideas 
the first idea swere like probably many a young developer what cool features i could add and how awesome it would be, planning so big that i could not realistically build it with my current skillset. After a walk to clear my head and a productive discussion with other software inclined friends i decided to go and build a V1/alpha first, a proof of concept. It just needs to work, but im still optimistic that i can write some code that will survive into future versions.

## technical decisions
the decision to support multiple databases even in the alpha was made to allow administrators to choose their database and even use already existing ones, for this purpose MySQY and Postgres were chosen due to their common usage. Docker and cubernetes are becoming the defacto default for application hostingfrom small homelabs to the datacentre and as such it only made sense to target them first and foremost

## Must have features 

The design of this bot is based aroud social pressure and helpful friends, as such the bot has a good amount of must have features:

User Features:
- Reminders
    - set reminders
    - modify reminders
    - delete reminders
    - snooze reminders
- Consent
    - consent to getting pinged by a user
    - remve consent to getting pinged by a user
- User Settings
    - set user timezone
    - change user timezone
    - set default dropped reminder behaviour
- Status

Server Admin Features:
- permitted channels
    - set permitted channel
    - remove permitted channel
- bot announce channel
    - set bot announce channel
    - unset bot announce channel

Bot Owner Features: 
- view bot logs
- manage bot
    - send messages to admins
    - set downtime 
    - restart bot
    - shut down bot

So, i think thats all for now, the only thing that is left now is to implement all these ideas.
In the next blog post ill be talking about more indepth design like program structure and database modeling, some of that work has already started but it still needs some light polish
