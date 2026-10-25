---
name: perfect-character
description: Generate any image or video of my approved character using the exact locked prompt, model, reference_id and parameters. Use whenever I ask for a new shot, scene or script of this character.
---

# Perfect character: Ellie (Higgsfield Model D)

Ellie is a disclosed AI character for Ameri-Vita. Every new image or video of her is built from the locked setup in `reference/golden-prompt.md`, so she looks like the same person every time.

Read before every job:
- `reference/golden-prompt.md`: the verbatim origin record (section A) and the locked production setup (section B)
- `reference/character-bible.md`: who she is, her look, wardrobe, voice and what never changes
- `reference/hero-still.md`: the hero still (master portrait) and where it lives

## Rules

1. **Always reuse the locked setup.** Use the model, reference_id (Element), hero still and identity-lock block from section B of `golden-prompt.md`, unchanged. Never swap the model, drop the Element or rewrite the identity-lock block.
2. **Only change the scene, action, camera and dialogue.** Face, hair, eyes, freckles, age, build and the phone-photo capture style stay as written. Outfit colour and accessories change only as the character bible allows.
3. **Show the cost first, then wait.** Before each generation, run `higgsfield generate cost` with the exact params (in the Claude app, use the Higgsfield connector's `get_cost: true` preflight instead). Show me the credits and wait for my explicit OK. No OK, no job.
4. **Log every generation.** After each job, append its job_id, date, model, final prompt and full params to `logs/generations.md`, newest at the bottom, using the template in that file.
5. **Never edit `reference/golden-prompt.md`** without my explicit approval in chat. If a change looks needed, propose the exact diff and wait.

## How to build a prompt

1. Start with the identity-lock block from section B, word for word.
2. Add the scene: one action in present tense, one setting with two concrete details, one named light source and its direction.
3. Add the camera: casual handheld iPhone photo, slightly off-centre, slight tilt, phone-sensor grain, background falling out naturally.
4. Add 2-3 real-camera flaws (flyaway hairs, fabric creases, handheld tilt).
5. For a product shot: first make an approved person-only frame, then add the product as an edit with its product Element (IDs in the bible).
6. For video: animate an approved still as the start image (settings in section B). Dialogue follows the voice rules in the bible.

Never write in her voice: first-person health results, before/after claims, reviews or endorsements. Product captions start with "Ad". British English throughout.
