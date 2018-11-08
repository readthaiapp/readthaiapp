---
layout: post
title: roadmap
permalink: "/roadmap"
---

This is the roadmap of the application, so all the new feature coming in in the next few weeks / months

## What's on the pipe! (Summary)

- Adding new sentences (I'd like to reach 1500 sentences end of the year)
- Let people add their own sentence/word in the app.
- Youtube/Instagram feed of curated content about Thai
- More games
- Adding the Dictionary and Translation service
- Switch to a better Text-To-Speech method
- Open the app, open the direct translator then show a picture with text with your camera and it automatically and instantly translate what's written.
- Account to save your profile online.
- Share space where users can speak together, share experience, tips, ask questions, etc
- Transform the app to be multi-level friendly (Beginner / Intermediate / Advanced)

## Adding new sentences

This will be progressive, I'll start to add 20+ sentences a day to reach that level of 1500 sentences end of the year (with some days where I'll put maybe 200 hundred in one time ;) )

I'll try to populate first the category which does not have a lot of sentences currently which are Feelings, Weather, Dating, Family.

## Let people add their own sentence/word in the app

I'll start with a first phase where people can add words only.

It's quite "hard" to put sentences in the app as I require many information per sentence.

Let's take an example:

    {
          "id": 110,
          "thaiSentence": "คุณใจดีมาก",
          "categories": [10, 11],
          "source": [1],
          "words": [54, 237, 84],
          "translations": {
            "english": "You are very kind."
          }
        },

That's what we have behind the scene for each sentence.

We can see that a sentence is divided by words (here 54,237 and 84).

If we look at 84 for example:

     {
          "id": 84,
          "word": "มาก",
          "tone": "F",
          "translations": { "english": "A lot" },
          "linkedWord": [],
          "synonym": [],
        },

A word have his definition in thai, a tone, a translation in english (that's the required minimum).

So for each sentence, I need to have a list of words which themselves need to have a translation & tone.

This is the simple case when the word only have one tone, but in case of a multi-tone words, the structure is a bit more complex.

I might be able to bypass that and so people will be able to add words/sentences without defining the tone but it means that those sentences won't be usable by the game section & displayed in search functionality when filtering on tone (for words).

The sentences have other mandatory info which are the category but by default we can say it's MISC.

Next to that, I would like to add the possibility to share the sentences created by users, so it will send it to me, then I'll correct them if necessary and add them after for everyone in the application.

## Youtube/Instagram feed

I've already written a blogpost about that so I won't repeat myself, but this is in my to-do list as I think it's very useful. There is really nice youtube video explaining the big concept of how to read Thai, or subtleties of the language.

## More games

On facebook, I saw someone interested in a kind of puzzle games which can be interesting to add in the app. Being able to play a bit more with the content is interesting.

Maybe also a game to teach ourself to type with the Thai keyboard.

## Adding Dictionary & Translation services

Right now, in the tools section, people can vote for the two. It seems that people would like to have that in-app, so will be it!

The issue with that is that it has a cost (backend) and I try to stay free as much as I can.  
I might add a payment system to become "Gold member" to access some of the feature of the app (the one which have a cost).

## Switch to a better Text-To-Speech system

Right now, I'm using the one built in the phone but the biggest issue is our friend from Samsung which does not have Thai language ... So it's really painful for our dear Samsung user to go in a configuration screen to change the language of that thing to the Google one.

Also, another Text-To-Speech system would be more voice type (Male / Female).

Android already let users choose between a male and a female but not iOS.

Again; this have a cost, so probably in a "paid" version of the app.

## Image/Text recognition

I've the ability to add that feature which I find really useful. Take your phone, scan through the camera a menu, a sign, or whatever containing Thai text, and you'll see the direct translation in english.

Again, this feature have a cost ( Quite expensive in fact ).

## Account to save profile online

When you have multiple devices and you want to share your favorite and soon your sentences/words between different device, we need to go through an online service to store that information.

This also have a cost; but relatively cheap

## A kind of "forum" in the app

A space where people can ask question, share an image, an advice, or other about Thai language.

## Multi-level friendly

Right now, the app is more for intermediate/advanced user.

I would like to add at the beginning of the app a kind of selection like

I'm a beginner / Intermediate / Advanced learner.

Depending on that, I could recommend a flow of sentences and technics to learn more effectively to read Thai.

# What do you think?

If you think that one of this idea need a bigger priority, or is wrong, or is super, or whatever it can be ;) Please comment down or send us an email.

We are reading all the suggestion so if you have something I didn't thought about yet, send it to us.
