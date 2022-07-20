---
template: post
title: Create a Todo List App with React
slug: todo-app-react-bulma
socialImage: /media/juanjo-jaramillo-mznx9429i94-unsplash.jpg
draft: true
date: 2022-07-20T15:52:11.475Z
description: An introduction to React by building a simple todo list app.
category: Web Development
tags:
  - React
  - Bulma
  - Javascript
  - Web
---
## Before We Begin

If you are just starting out with creating apps in *React*, then you may be looking for a good first project to help you learn the ins and outs of the framework. Building a todo list app is a perfect way to introduce yourself to the basic concepts of *React* while creating something that you can show off to others. 

This article assumes that you have a basic understanding of HTML and Javascript and already have a folder with a fresh install of *React* in it. If not, you can check out this [simple guide](https://blog.conrad-king.dev/placeholder) on how to set things up.

## First Things First

If you're not familiar with component based web frameworks, _React_ may come as a bit of a shock to you. Historically, interactive websites and web apps have kept their page structure (_HTML_) and behavior (_Javascript_) in separate files (unless you use `<script>` tags, in which case don't talk to me). _React_ and other frameworks marry these two aspects in what are called _components_.

Components look a lot like regular HTML elements that you may be familiar with, such as `<div>` or `<span>`, but have a few more tricks up their sleeve that we will go over. Here is an example of what a _React_ component looks like in markup:
```
<Hello name={"Conrad"} />
```

