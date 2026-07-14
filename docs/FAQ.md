# FAQ

## What is this repository?

This is a source-backed public collection of Nano Banana prompts, prompt skills, visual examples, and attribution metadata.

It is an independent community repository, not official Google documentation. Model capability statements in the README should be tied to official Google docs.

## Which model does “Nano Banana” mean here?

This repository uses the original model name only: Nano Banana is Gemini 2.5 Flash Image, model code `gemini-2.5-flash-image`. Google documents it as a native multimodal image model for text-and-image input, text-and-image output, high-volume generation, and conversational editing. It produces 1024px-class images and generated images include SynthID.

Nano Banana 2, Nano Banana 2 Lite, and Nano Banana Pro are separate models. Their prompts and capability claims are outside this repository's scope.

## Is the original Nano Banana still Google's recommended default?

No. Google now describes it as the legacy pioneer of the family and recommends newer Nano Banana models for new workloads. The collection remains useful for people who still run `gemini-2.5-flash-image` and want source-backed workflows rather than inflated claims.

## Where does the data come from?

Maintainers can collect candidates through local tools, manual curation, or community GitHub Issues. Approved entries are normalized into the same prompt data shape and rendered into README files.

## Does this repo require an external service?

No. README generation uses local structured data in this repository.

## How do I submit a prompt?

Use the **Submit a Prompt** GitHub issue template and include the prompt text, generated images, author, source link, and language.

## Why are there many README files?

The published prompt remains in its source language so readers can verify it against the creator's post. Every non-English README has its own reviewed title and description for each entry, localized interface copy, workflow explanations, and matching ImagineVid route. The prompt block is explicitly labeled as the original English text rather than presented as a translation.

## How do removal requests work?

Open an issue with the affected source link and the requested action. Maintainers will remove or update the entry.
