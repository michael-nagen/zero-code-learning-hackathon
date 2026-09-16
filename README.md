# The Orange Project

> A hackathon proof of concept for making high-quality learning possible at scale — even for people with zero technical skills.

## The idea

The Orange Project explores a **zero-code learning experience**: a learner can download an open AI model and the learning software locally, then use the system without relying on a paid, closed AI service. The goal is not to deliver a finished product or a programming course; it is to demonstrate that this learning model can work broadly for people starting from zero.

## What the concept demonstrates

- **Local-first AI:** learning experiences can run with downloadable open models and free local software.
- **Accessible by design:** the learner does not need programming knowledge to use the system.
- **Adaptive instruction:** lesson content and tutor behaviour are shaped around the learner and the teaching goal.
- **A scalable direction:** the model is intended as a starting point for broader, lower-barrier education.

## My contribution

Beyond the visual dashboard, I designed and implemented the orchestration layer behind the learning experience. It processes lesson material, learner context, and teaching objectives to build an instructional plan.

The orchestration decides how to structure the lesson and the tutor, and selects the appropriate prompt for the specific learning situation. In practice, that means turning the question “what is the best lesson and teacher for this learner right now?” into a controlled workflow rather than a single generic prompt.

## Prototype scope

This repository is a hackathon prototype and a product exploration — not a finished learning platform. The included React dashboard demonstrates the interface and interaction model for organizing learning tools. Production integrations, persistent learner data, authentication, and local model runtime are intentionally outside the current scope.

## Technology

- React 18
- TypeScript
- Vite
- React Router

## Run locally

```bash
npm install
npm run dev
```

For a production build:

```bash
npm run build
npm run preview
```

## Next steps

- Connect the orchestration layer to a local open-weight model runtime
- Add learner profiles and persisted learning progress
- Evaluate lesson and tutor strategies with real learner feedback
- Turn the hackathon proof of concept into a complete learning product
