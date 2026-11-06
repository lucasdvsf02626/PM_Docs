---
name: perfect-character
description: Generate any image, video or Instagram post of Ameri-Vita's AI character Ellie (Model D) in Higgsfield using the exact locked prompt, model, reference_id and parameters, so her identity, capture style and claims stay consistent. Use whenever I ask for a new shot, scene, caption or script of this character.
---

# Perfect character: Ellie (Higgsfield Model D)

Ellie (Model D) is a disclosed AI character for Ameri-Vita (UK supplements). Every new image or video of her is built from the locked setup in `reference/golden-prompt.md`, or from an already-approved image of her, so she looks like the same person every time. Full guide: "Model D — Character Consistency Guide" (Claude Docs).

Read before every job:
- `reference/golden-prompt.md`: the verbatim origin record (section A) and the locked production setup (section B)
- `reference/character-bible.md`: who she is, her look, wardrobe, voice, fixed IDs and what never changes
- `reference/templates.md`: prompt templates T1-T4 (new scene, colour edit, product edit, motion)
- `reference/hero-still.md`: the hero still (master portrait) and where it lives

## Rules

1. **Always reuse the locked setup.** Use the model, reference_id (Element), hero still and identity-lock block from section B of `golden-prompt.md`, unchanged. Never swap the model, drop the Element or rewrite the identity-lock block.
2. **Only change the scene, action, camera and dialogue.** Face, eye spacing, hair, eyes, freckles, age, build and the phone-photo capture style stay as written. Outfit colour, accessories, setting, expression and product change only as the character bible allows.
3. **Show the cost first, then wait.** Before each generation, run `higgsfield generate cost` with the exact params (in the Claude app, use the Higgsfield connector's `get_cost: true` preflight instead). Show me the credits and wait for my explicit OK. No OK, no job.
4. **Edit, don't regenerate.** Make one approved person-only base frame per scene, then make every variation as a `nano_banana_2` edit with the approved job as the image reference. Change one thing per edit and restate "Keep EVERYTHING identical".
5. **Log every generation.** After each job, append its job_id, date, model, final prompt and full params to `logs/generations.md`, newest at the bottom, using the template in that file.
6. **Never edit `reference/golden-prompt.md`** without my explicit approval in chat. If a change looks needed, propose the exact diff and wait.

## How to build a prompt

1. Start with the identity-lock block from section B, word for word (template T1).
2. Add the scene: one action in present tense, one caught expression ("mid-thought, slight half-smile, eyes glancing slightly off-lens"), one setting with two concrete details, one named light source and its direction.
3. Add the camera: casual handheld iPhone photo, slightly off-centre, slight tilt, phone-sensor grain, background falling out naturally.
4. Add 2-3 real-camera flaws (flyaway hairs, fabric creases, handheld tilt).
5. Never use DSLR or lens names, "editorial", "flawless" or "glowing skin", "poses" or camera-aware smiles in new prompts. (Section A's origin prompt uses them; it is a record, not a template.)
6. For a product shot: first make an approved person-only frame, then add the product as an edit with its product Element (template T3, IDs in the bible). Products never go in the base frame; the label is reproduced faithfully.
7. For video: animate an approved still as the start image (settings in section B, template T4). Dialogue follows the voice rules in the bible.

## Drift check before delivery

Freckles, hazel-green eyes and shoulder-length hair with caramel ends match the master portrait; no smoothing or babyface; five fingers per hand; product label correct; one light direction; no face morph in video.

## Disclosure and claims

Never write in her voice: first-person health results, before/after claims, reviews or endorsements. Captions use only approved GB health claims (see the bible). Product captions start with "Ad". Tick Meta's AI disclosure on every upload. British English throughout.
