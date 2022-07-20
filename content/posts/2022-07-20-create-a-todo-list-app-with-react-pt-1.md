---
template: post
title: Create a Todo List App with React, Pt. 1
slug: todo-list-react-1
socialImage: /media/juanjo-jaramillo-mznx9429i94-unsplash.jpg
draft: true
date: 2022-07-20T17:27:49.716Z
description: Getting your feet wet with React by creating a Todo List app.
category: Web Development
---

![](/media/juanjo-jaramillo-mznx9429i94-unsplash.jpg)

## Before We Begin

If you are just starting out with creating apps in **React**, then you may be looking for a good first project to help you learn the ins and outs of the framework. Building a todo list app is a perfect way to introduce yourself to the basic concepts of **React** while creating something that you can show off to others.

This article assumes that you have a basic understanding of HTML, Javascript and already have a folder with a fresh install of **React** in it. If not, you can check out this [simple guide](https://blog.conrad-king.dev/setting-up-react) on how to set things up.

## A Quick Dip into React

### Components Overview

If you’re not familiar with component based web frameworks, **React** may come as a bit of a shock to you. Historically speaking, interactive websites and web apps have (almost) always kept their page structure (*HTML*) and behavior (*Javascript*) in separate files. **React** and other frameworks allow you to break a web app down into composable pieces called **components** that are responsible for both their own structure and behavior.

Components look a lot like regular HTML elements that you may be familiar with, such as `<div>` or `<span>`, but have a few more tricks up their sleeve that we will go over. Here is an example of what a **React** component looks like in markup:

```
<Hello name="Conrad" />
```

What are we looking at exactly? Well, `Hello` is the name of this component, while `name` is an attribute (or property, when talking about components) of `Hello` with the value of `"Conrad"`. When this component is rendered (ie. displayed in a browser), a function by the same name of the component is called with all of its properties passed in an argument object. The result returned from that function is then processed by *React* and spit out onto your web browser. 

Let's look at a more concrete example of this in action:

<iframe height="350" style="width: 100%;" scrolling="no" title="Untitled" src="https://codepen.io/RainbowReich/embed/preview/oNqWZqX?default-tab=js%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="false" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/RainbowReich/pen/oNqWZqX">
  Untitled</a> by Conrad King (<a href="https://codepen.io/RainbowReich">@RainbowReich</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

Ok, let's break this down. The `Hello` function is what drives the `Hello` component's behavior. When it's rendered, it takes the `name` property from the `props` argument and places it inside of a `<div>`. That `<div>` then gets returned and sent to *React*.

You're probably a little confused right now. Why is there HTML smack-dab in the middle of my Javascript function? Why is there a Javascript variable smack-dab in the middle of my HTML? How do both of these languages cooperate with eachother? These questions can be answered by a little something called **JSX**.

### JSX Overview

**JSX** stands for _Javascript XML_, and is what allows us to mix Javascript and HTML when working with React.