---
title: "Moving from React to Svelte"
date: 2026-05-23 00:00:00 +0000
categories: [development, frontend]
tags: [svelte, react, migration, ui]
---

In 2023, I started working at Angel One. Until that point in my career, I had worked primarily with React. The stack I was supposed to lead was built on Svelte and SvelteKit.

This post is about my journey of moving from React to Svelte, the mindset shift involved, and what I learned while trying to build scalable UI systems with it.

React is a very component-driven framework. Everything you build becomes a component. Even props can be components. State management is also very explicit. There is a clear way to update state, and the rendering flow feels predictable.

You build components, pass props, compose children, and customize behavior through composition. Passing components as props is incredibly powerful and solves many customization problems elegantly.

Another major shift React introduced was writing JavaScript directly inside HTML. Once you start building frontend applications this way, it becomes difficult to go back to traditional templating approaches.

This is where Svelte felt very different.

Before Svelte 5, state changes were much less explicit. Any variable could become reactive. Initially, this felt magical, but also slightly uncomfortable coming from React.

Children composition also worked differently through slots. Slots are a great way to keep component trees predictable, but coming from React, they initially felt restrictive.

In React, I was used to deeply composable component patterns where almost everything could be overridden or customized. Building wrappers around functionality was natural and extremely flexible.

That mindset does not translate directly into Svelte.

Another major shift was CSS. In Svelte, component styles are scoped by default and do not leak into child components. This keeps styling much cleaner, but adapting to that model after years of React development required a mindset change.

Understanding how to structure nested styling and reusable UI patterns took time. As a dev who loves to style using css mostly this was a hard pill to swallow.

Migrating to Svelte was difficult, and I do not think that part ever completely changes when moving between frontend ecosystems.

But there were clear benefits. The biggest one was simplicity.

Our use case required a platform that was lean and low in complexity, and Svelte fit that extremely well. Most pages required fewer lines of code, less boilerplate, and less framework overhead.

Once I became comfortable with Svelte’s reactivity model, building reactive interfaces started feeling very natural.

One challenge in the early days was third-party ecosystem support. React still has a much larger ecosystem, but Svelte has evolved significantly over the past few years, and support today is far better than it was when I started.

One thing I appreciated about Svelte is that it pushes you toward simpler solutions.

In React, it is easy to build highly abstracted components with increasingly complex state management. Svelte, in many ways, encourages you to simplify both the component structure and the state flow.

That does not mean the problems are less complex. It just changes how you approach them.

There are still days when I miss the flexibility and ecosystem of React.

I miss passing components as props to solve customization problems. I miss some of the patterns and hooks that make React development feel structured and extensible.

But Svelte has its own philosophy and way of solving problems.

And after spending the last three years working with it, I can confidently say that the approach is not wrong — just different.

The biggest shift was not learning Svelte.

It was unlearning how I thought about frontend architecture while using React.
