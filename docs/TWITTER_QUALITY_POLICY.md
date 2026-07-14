# X Source Review for Original Nano Banana

twitterapi.io is a discovery tool, not a publication pipeline. A keyword match can surface reposts, newer Nano Banana family models, engagement bait, prompt fragments, or images created by another tool. Nothing enters `data/prompts.json` directly from search output.

## Discovery Pass

Searches should cover both the public nickname and the model identifier:

- `"nano banana" prompt`
- `"gemini 2.5 flash image" prompt`
- focused workflow terms such as edit, reference, typography, product, storyboard, map, restoration, or architecture

Queries for newer family names are used only as exclusion checks. Raw responses stay in the ignored `data/research/` directory.

## Source Reconstruction

For each candidate, inspect the complete public context:

1. Start with the original post and confirm its author.
2. Follow the author's replies when the post says “prompt below” or “prompt in thread.”
3. Read image ALT text when the prompt is stored there.
4. Inspect quoted posts to distinguish the prompt author from the person sharing a result.
5. Record the exact prompt location in `sourceMeta.prompt_source`.

If the public thread does not contain the full prompt, reject the candidate. A plausible reconstruction is not provenance.

## Admission Gates

An entry must satisfy every gate:

- explicit evidence for Nano Banana or Gemini 2.5 Flash Image;
- no explicit Nano Banana 2, Nano Banana Lite, Nano Banana 2 Lite, or Nano Banana Pro targeting;
- canonical `x.com/{creator}/status/{id}` source;
- original creator attribution;
- complete reusable prompt text;
- visible source result media;
- exactly one primary workflow category;
- honest prompt-location metadata;
- no exact or perceptual duplicate in the published collection.

## Quality Ranking

The scorer prioritizes complete prompts, visible results, author identity, and useful engagement signals. Its `accept` decision means “inspect first,” not “publish automatically.” Manual review may reject a high score when the post mixes models, hides the prompt behind a private message, or presents generic promotional material.

## Duplicate Boundary

Before publication, compare:

- tweet and source IDs;
- normalized prompt text;
- canonical media URLs;
- perceptual hashes of downloaded public media.

Visual duplicates are merged into one source-backed entry. Minor caption changes, crops, or reposts do not justify a second item.

## Publication Record

Published entries retain the search provider, root tweet ID, prompt tweet ID when applicable, prompt location, model evidence, engagement snapshot, and collection date. This record makes later corrections possible without exposing API credentials or committing raw search caches.
