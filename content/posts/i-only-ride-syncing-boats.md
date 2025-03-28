---
title: 'I only ride syncing boats'
date: 2025-03-27T20:57:42+02:00
draft: false
---

# What does it mean a "syncing" boat

As it sounds, you go on a boat and you sync yourself to whatever the status of the boat is.
You might be building the boat yourself or you might hop onto one of your colleague's boats, but you never observe carefully before or during the sail—you simply sync yourself to the boat you are on.

If it roams the high seas at tremendous speeds and you feel the wind through your hair, you sync to that.
If the boat is calm and doesn’t move fast, you don’t open the sails or change direction to the wind—you just allow yourself to float on the sea to no end and let the tides take you.
And of course, if the boat **sinks**, you sync and you sink with the boat.

# But what does it have to do with software

Say, dear developer reading this (or normal person who touches grass once in a while), have you ever been assigned to a project where you actually knew the status of the project?

The real status—not the bullshit the product manager says to the higher-ups via PowerPoint slides.
Either the project is a nightmare to work on, and the amount of technical debt is so large it’s more likely the US will pay off its debt first,
OR maybe it's a successful project, or an app where you fix bugs from time to time, and sometimes they ask you to add a feature so small it’s like wrapping ChatGPT and adding “Do not hallucinate” to the prompt as _“innovation.”_

## So you know the feeling?

If you don’t, then you are either blessed… or the product manager.

If you do, I believe you’re like most of us: added onto the project, trying to understand as you go what you should think about it, how you should talk about it during daily meetings or lunch breaks, and of course—how to code in it.

# But I hate boats

Yes, I really do. But I keep going on them—even if they sink right in front of my eyes.

Let me give you two examples I’ve personally experienced:

1. A React app that had components with around 1500 lines each, about 50 `useState` in each component, and a `useEffect` that was just 500 lines long.

2. An app I’m solely responsible for that crashes regularly due to the fact it may request 1GB of data every minute.

## The first boat

I was assigned to a project after another developer left the company.
It was the first real project I got to handle (in my first job), so I wanted to impress. I was ready to put in the blood, sweat, and tears necessary.
I remember thinking to myself that I finally get to see industry-level source code—it must be handled nicely with good CI/CD and an organized project structure.

That thought was shot dead so unmercifully that it didn’t even get a funeral until I wrote this post.

The code was just so hard to follow. The components were too long to understand and follow.
So me, a new developer, thought to myself: this needs a major refactor.
I went to my boss and told him how I see things, and he told me that it’s fine and to simply allocate more time to understand the flow of the project.
“It’s **fine**,” he says.
Is it **fine**?
Well, he’s my boss and has more experience than me, so… it’s **fine**.

It was, in fact, not fine. And I knew it wasn’t fine.
But I boarded the boat.

And I was in sync with the boat the whole way. I hacked my way through problems I knew were technical debt, but I delivered the product, so it was still fine.
I kept going the way my predecessor went and kept adding `useState` like there was no tomorrow. Some components ballooned to over 2000 lines.
But the PRs were approved, so it was fine.

I was in sync with the boat.
I let the boat’s tide take me wherever it wanted. And while I knew it hadn’t sunk yet, when it does—I will go down with it.

## The second boat

This app I started from scratch, so I knew I could put in the work to add structure and order to the code so that me and others would be happy to work on it.

Everything in the app was great—except one thing: the data fetching.

The app is a dashboard widget for another service. We put the app on its marketplace, and due to the nature of a dashboard, you need to request all of the relevant data to display something meaningful.
So my solution was: just bring all the data and... profit?

So what if it might be mountains of data? Modern computers are fast and can handle it!
In testing, the app failed to load only 2% of the time—who would even notice?

My thoughts were that since the project is well-structured, it would be easy to fix the problem later.

And while that thought wasn’t shot dead, it is currently being held hostage as I write this.

The app was considered pretty good and even got a small award on the marketplace.
I was happy with my work and left the known problem for future-me to solve, while I kept adding features to what I considered my success story.

The app continued to grow and add more features, which in turn added more data to fetch.
Now it fails about 10% of the time right at the start, which causes rage clicks that bring in even more data, spiraling out of control.
It got so bad the API team of the company contacted us and said they’d shut the app down if we don’t fix it.

The boat had leaks all around, and the boat was roaring through the seas.
I chose to sync to the roaring, and now I sync with the sinking—because I won’t be able to fix the problem in time, and the app will be shut down.

# Why do I hate boats

Because they make me sick

# What do I hate about the way I develop software

I hate that the direction of a project goes by the whims of external forces, and that they are not steered correctly using those forces.
In the end, I and the people I work with write the code.
We are the builders, the navigators, and the captains of each part we develop or fix. Yet it always feels like we are out of control of the real situation.

We must accept the fate, and we must sync to whatever those forces may be—whether it’s the force of a user or a boss, we will abide, and the boat will steer (or sink) in that direction.

Most of the time, it feels more like being on a ramp than being on a boat, because for some of the time, you truly don’t have control over what you will write—even when you know there are more important matters than whatever the current task is.

# So why don't you stop boarding boats?

I have a wife and a baby and I would prefer they will have a nice house and food on the table.

## Didn't you stop with the metaphors?

Nope, Because I think it is a good one.

# What should I change

- I shouldn't be afraid to call out problems I know are there. And I should keep the forces in bay and use them when I need to.

- Fix leaks when you see them, and ignore people who say that the leaks are not there.

# What's next

I will rise from the seas from the boats that have sunk, find a shore and will most likely board a new boat. But before I board I will at least check I brought a compass
