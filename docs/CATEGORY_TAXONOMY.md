# Nano Banana Workflow Taxonomy

This collection classifies a prompt by the creative decision that makes the original Gemini 2.5 Flash Image workflow useful. A portrait is not automatically a character prompt, and a four-panel image is not automatically a storyboard. The primary category follows the job being done with the model.

## The Six Workflow Families

### Directed Editing & Input Control

Use this when supplied visual material is essential to the instruction. Typical signals include preserving identity, restoring a photograph, changing one region, transferring a subject into a new setting, or combining references while keeping specific details stable.

### Commercial Design, UI & Posters

Use this for deliverables that must communicate: advertisements, campaign systems, brand marks, packaging studies, interfaces, editorial layouts, typography-led posters, and reusable product-photography setups.

### Diagrams, Technical Art & Storyboards

Use this when information order matters more than a single hero image. It includes cutaways, specification sheets, maps, model sheets, exploded views, annotated boards, and sequences whose panels carry distinct roles.

### Characters, Cinema & Visual Styles

Use this for a visual identity, character treatment, portrait language, cinematic frame, fashion direction, or repeatable rendering style when none of the more task-specific groups is the main purpose.

### Environments, Architecture & Worldbuilding

Use this when the place carries the concept: landscapes, rooms, buildings, travel scenes, environmental concepts, and fictional worlds whose spatial design is the central result.

### Benchmarks & Model Comparisons

Use this only for controlled evaluation. The entry must identify what remains fixed, what changes between runs, and which behavior is being compared, such as text rendering, edit fidelity, identity preservation, or composition.

## Classification Questions

Ask these in order:

1. Is the entry a controlled evaluation rather than a showcase? Choose **Benchmarks & Model Comparisons**.
2. Would the prompt lose its purpose without an uploaded image or explicit edit target? Choose **Directed Editing & Input Control**.
3. Does the result depend on ordered panels, labels, measurements, or explanatory structure? Choose **Diagrams, Technical Art & Storyboards**.
4. Is the requested output a usable communication or brand asset? Choose **Commercial Design, UI & Posters**.
5. Is the location or built environment the principal subject? Choose **Environments, Architecture & Worldbuilding**.
6. Otherwise, choose **Characters, Cinema & Visual Styles**.

Every prompt receives exactly one primary workflow. Searchability must come from a clear taxonomy, not from assigning the same entry to every plausible category.
