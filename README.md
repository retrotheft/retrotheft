# Hello there 👋

I'm Jim, an open source developer from Melbourne, Australia. In a previous life I was an avid Svelte developer, but have turned to the dark side and am now all in on Effect-ts and Foldkit, which I was surprised to find actually make agentic development very viable - something I was very sceptical about until mid 2026, despite having used AI for several years before that.

As it turns out, several of the things I was working on by hand turn out to be incredibly useful for agentic development. Most of my current projects involve solving issues that coding with AI brings with it. Several of these I use in my day to day workflow, and are getting quite close to release, I swear.

## Projects

### Together

This app is the only reason I'm able to work on all of these projects simultaneously and effectively. It's a project manager that facilitates interactions between Human and AI tasks. I've seen plenty of Software Factory / Swarm Manager approaches, but all of them look too much like a black box to me. Together displays tasks organised by whose responsibility they are, uses interactive Markdown reports for seamless Human actionability, lets you create Arcs so you can keep track of where you're headed, manages your session history and provides recommendations on what work to do next. It also has a cool graph view.

### Selectoplasm

One of the biggest headaches with agentic development is UI work and iteration. Man, really, it's horrible. Fortunately it turns out I accidentally built a solution to this in 2024 without realising it, before I even used AI much. (I think I was using Github Copilot at the time. Remember Github Copilot?)

Selectoplasm allows you to completely externalise your styling from your app. It provides a way for an AI agent to interact with your UI and make changes that are completely reversible and replayable. And not just that - the state history is composable, so you can view any element at any time, against any other element at any time.

It also provides a better division of labour - instead of asking the AI to change a font, you ask the AI to load a range of fonts into your interface, that you can then switch between in realtime. Essentially, it uses workflow latency as a measure of where the demarcation should be between what you do, and what the AI does. Actually, I think that's a running theme in a lot of my projects.

### Casca

What if, like, Tailwind was its own LANGUAGE, man?

Casca originated as the emmet-inspired syntax that Selectoplasm was built on. It wasn't until two years later that I realised it should be its own thing. Essentially, Casca collapses both HTML and CSS into a one-dimensional markup language. This is incredibly powerful and agents seem to love it. It lets you do things like replay any changes to your website in realtime, express your component libraries, brand utilities, and design systems in simple readable files, and since HTML and CSS can be derived from Casca, it's framework agnostic, so you can scaffold a fully built website to any framework. It also makes advanced CSS concepts like Lea Veroux's [pseudo-private custom properties](https://lea.verou.me/blog/2021/10/custom-properties-with-defaults/) first-class citizens, so styling composability is a breeze.

### Improv

Improv is a tool for maintaining code quality through constructive data modeling and claim fingerprinting. It derives Claims from your authored spec, and refactors the code so that every Claim has a reified outcome, which is very often just the success or fail case of a Result. Combined with Effect-ts, this process is great at improving code readability, semantic intent, and at finding and correcting bugs before they happen. It also delivers a comprehensive derived spec which you can use as the window to your app, without needing to read the code. Every Claim is fingerprinted using a hash, so if the code changes, it's visible, and using this, agents can track not just when code changes, but also when code changes that shouldn't really be related to another claim, helping reduce complection.

### Riley the Roleplay Engine

This started as a fairly simple LLM roleplay app, but has become its own architecture - Oracle at the Gate - which is probably worth writing a paper about. It's a deterministic workflow engine that works with YAML files called Frames that can define an entire app's worth of behaviour. Its goal is to significantly reduce the reliance on LLMs for work that we should really still be doing deterministically. You know, programming. And yes, I am integrating Zev into it right now.

### Substrate

Substrate is my internal tool for identifying shared code opportunities between my projects. It currently consists of my UI Kit and AI Services.

---

> A big thankyou to [epicenter](https://github.com/epicenter-so/epicenter) for sponsoring my open source work! Epicenter is an ecosystem of open-source, local-first apps, whose vision is to build a personal workspace where you own your data, choose your models, and replace siloed apps with open, interoperable alternatives. All while preserving authenticity and being free and open source.
