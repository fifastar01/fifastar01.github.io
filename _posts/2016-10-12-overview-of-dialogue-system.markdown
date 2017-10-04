---
layout:     post
title:      "Overview of dialogue system"
subtitle:   "How to design a chatbot, part one"
date:       2016-10-12
author:     "Dennis"
header-img: "img/post-bg-2015.jpg"
tags:
    - Dialogue System
    - Chatbot
    - AI
---

## Dialogue and Dialog System
People engage in dialogues all day long and few people thought about why they converse with others. Dialogue is a collaborative activity to fulfill specific goals. It can be used by human or computer programs to :

* exchange ideas
* request information
* sustain relationships

For a natural conversation, there are some major characteristics of a dialogue: 

1. Turn-taking
2. Coherent interactions
3. Multiple modalities

![][image-1]

Dialog system is a computer system intended to converse with a human, with a coherent structure (definition from [wikipedia][1]).

## When is dialogue system useful?

Compared with graphic user interface, there are some scenarios that conversation user interface is more convenient.

1. When hands-free interaction is needed such as in-car interface,  intelligent household and command-and-control interface

2. When natural interaction is more efficient such as voice search, virtual assistant, VR etc

3. When human costs can be greatly reduced like call routing, customer services and selling Q&A

## Examples of dialogue system

![][image-2]

Apple Siri, Microsoft Cortana, Google Assistant, Amazon Echo, Facebook M and Baidu Duer are some famous examples of personal assistant dialogue system. Laiye is a start-up in similar position with strong technological expertise. 

## Components in dialogue system

![][image-3]

There are five components in dialogue system: Automatic speech recognition(ASR), Natural language understanding(NLU), Dialogue management(DM), Natural language generation(NLG) and Text-to-speech synthesis(TTS).

In specific,  ASR maps raw speech signal to a set of recognition hypotheses for user utterances. NLU maps recognition hypotheses to high-level semantic representations such as entities and user intent. DM updates the dialogue state and decide what actions to perform. NLG finds the best linguistic realization for the selected actions. Finally, TTS synthesize an audio signal out of the generated utterance.

## Evaluation of dialogue system

The performance of dialogue system is difficult to evaluate. What is the best way to evaluate bots has been a heated topic among academics and industry. 

For task-oriented bots, it is relatively easy since the task is based on tagged data. For each components, bot can be evaluated by metrics such as precision rate and recall rate. As a whole, the dialogue bot can be evaluated by successful task completion rates. Though in many cases, the completion of the task depends on many factors apart from bot design.

For chat-oriented bots, the task is usually more open end. Bots design usually borrow evaluation metric like BLEU from machine translation.

The main problem is for all evaluation methods is that its effectiveness depends on good human judgement. In many cases, securing high quality data can be challenging to reach objective results.


[1]:	https://en.wikipedia.org/wiki/Dialog_system

[image-1]:	{{ site.baseurl}}/img/over_sys/test_con.png
[image-2]:	{{ site.baseurl}}/img/over_sys/dia.png
[image-3]:	{{ site.baseurl}}/img/over_sys/dia_com.png