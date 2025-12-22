# UltimaCore ⚡

UltimaCore is a lightweight Python orchestration library that enables multiple AI models to collaborate, review, and improve each other’s outputs.

It is designed to make multi-model teamwork simple, fast, and accessible — even for non-experts.

---

## Why UltimaCore?

Most AI tools work like this:

One prompt → One model → One response

Real problem-solving doesn’t work that way.

UltimaCore introduces a team-based AI approach, where multiple models work together — just like humans in a team.

---

## Core Idea

UltimaCore allows multiple AI models to:

- Receive the same input
- Generate independent responses
- See each other’s outputs
- Review, discuss, and improve results together
- Produce a stronger final answer

All of this happens automatically.

---

## Installation

pip install ultima-ai

(Note: package name may be finalized during initial release)

---

## Basic Usage (Beginner-Friendly)

from ultimaai import UltimaCore

result = UltimaCore.asyncio(
    models=[model_a, model_b],
    prompt="Design database schema"
).run()

print(result)

That’s it.

- No async code
- No complex setup
- No framework knowledge required

---

## What This Does

- Runs multiple models in parallel
- Allows models to see each other’s outputs
- Enables natural, free-form collaboration
- Returns a unified final result

UltimaCore handles all orchestration internally.

---

## Design Principles

UltimaCore is built on three strict principles:

1) Simplicity First
- One function
- One prompt
- One result
- Even non-coders should be able to use it

2) Model-Agnostic
- No dependency on OpenAI, Google, or any single provider
- Works with any model or API the user supplies
- You bring your own models

3) Speed Matters
- Lightweight
- Async-powered internally
- Scales from 2 models to many (user-controlled)

---

## Advanced Control (Optional)

By default, models collaborate freely.

For users who want structure, UltimaCore supports optional role-based coordination:

UltimaCore.roles.asyncio(
    coder=model_a,
    reviewer=model_b,
    prompt="Optimize this algorithm"
).run()

Freedom by default.
Structure when needed.

---

## What UltimaCore Will NEVER Do

- Lock users into a specific API provider
- Hide outputs between collaborating models
- Force complex abstractions or deep async knowledge

---

## What UltimaCore Always Guarantees

- Models can collaborate openly
- Fast execution
- Clean, readable usage
- User control

---

## Project Status

Early-stage open-source project.

Core ideas, API design, and orchestration logic are being finalized before implementation.

---

## Maintainer

Hardik Sen
Founder, Master AI  
India

---

UltimaCore is an experimental orchestration library.
APIs may evolve as real-world usage informs improvements.
