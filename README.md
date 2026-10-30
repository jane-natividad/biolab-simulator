# BioLab Simulator

Run simulated growth experiments on fictional strains, compare scenarios and see exactly why the curves differ.

**[Try the live demo](https://biolab-simulator.vercel.app)**. It works straight away with no setup, runs entirely in your browser, and stores nothing. All data is fictional or synthetic.

## Why I built it

Growth experiments blend three things: the organism, the conditions and the noise in measuring them. I wanted a bench where each can be changed on its own, so it's always clear why one curve ends up higher than another.

## The problem

Experimental results blend biology, conditions and noise, so it's hard to tell which assumption made one strain look better, or whether a difference is real at all.

## What I built

A virtual lab built on logistic growth, solved numerically, with clearly documented nutrient and environment effects and an optional mode for nutrient depletion and product formation. It includes simulated replicates, a baseline comparison that explains why results differ, five preset experiments, a run history and a two parameter explorer.

## Who it's for

R&D, bioprocess and product teams, and anyone learning experimental design.

## What it does

- Choose fictional strains and edit their growth rate, capacity, nutrient response and tolerance
- Set starting population, nutrients, a neutral condition index, measurement noise, duration and replicates
- See growth curves, final and peak population, time to threshold and estimated versus true growth rate
- Set a baseline and get a plain explanation of why a new run differs
- Run five preset trade off experiments, save runs and overlay them
- Explore two parameters at once with a heatmap and a sensitivity chart

## Decisions that shaped it

1. **Honest about biology:** the environment is a neutral 0 to 1 index, never labelled temperature or pH.
2. **The equations are on the page:** everything is written out in the model card.
3. **Honest variability:** replicate spread is measurement noise, and estimation bias is visible.

## Key takeaway

The environment is a neutral index, replicate bands show measurement noise only, and the estimated growth rate sits beside the true one.

## Built with

- HTML, CSS and JavaScript in a single file
- A seeded random number generator, so every run is reproducible

## Run it locally

Open `index.html` in any browser. There's nothing to install.

## About this project

This is a working prototype I built to explore a real problem space. It uses illustrative, fictional data and isn't connected to any organisation's systems. You can find more of my work at [jane-natividad.github.io](https://jane-natividad.github.io).

Built by [Jane Natividad](https://github.com/jane-natividad).
