# Prompt templates

All templates use the default Element `e9783c1f-0669-4d38-b14c-df17b3403e07` (v2) from `golden-prompt.md` section B. `[IDENTITY-LOCK BLOCK]` means the section B block pasted word for word.

## T1 new scene still

`nano_banana_2`, 2k, 4:5 (feed) or 9:16 (Reels/Stories). Person only: no products.

```
Casual handheld iPhone photo of [IDENTITY-LOCK BLOCK], [ACTION], [CAUGHT EXPRESSION]. [SETTING + 2 concrete details]. [ONE LIGHT SOURCE + direction]. She wears [OUTFIT], [ACCESSORIES]. Slightly off-centre, slightly imperfect framing, slight handheld tilt, background falling out naturally as in any phone photo. Phone-sensor grain, visible skin pores, flyaway hairs, fabric creases. Realistic hands and fingers. No retouch, no smooth-skin filter. No text, no logos, no products.
```

## T2 colour edit

`nano_banana_2` edit; image reference = the approved base frame job.

```
Edit the reference photograph. Keep EVERYTHING identical: the same woman <<<e9783c1f-0669-4d38-b14c-df17b3403e07>>> with the same face, freckles, hair, pose, hand position, expression, camera angle, framing, background and daylight. Change ONLY the colour-matched outfit and accessories: [COLOUR] [TOP], small [COLOUR] drop earrings, a [COLOUR] claw clip in her hair. Photorealistic, natural colour grading. No text, no logos, no products.
```

## T3 product edit

`nano_banana_2` edit; image reference = the approved person-only frame; product Element from the bible.

```
Edit the reference photograph. Keep EVERYTHING identical: the same woman <<<e9783c1f-0669-4d38-b14c-df17b3403e07>>>, the same face, hair, camera position, framing, background and daylight. Change ONLY: [PRODUCT PLACEMENT with <<<PRODUCT_ELEMENT_ID>>>], label facing camera and reproduced faithfully with no changes to label, cap or packaging. Realistic hands and fingers, natural grip. Photorealistic. No added text.
```

## T4 motion

`kling3_0`, settings from section B, `start_image` = an approved still.

```
The woman stays in the same position. Natural, subtle real-world movement: [2-3 SMALL ACTIONS]. Gentle breathing, natural blinks. The phone camera is completely locked: no zoom, no pan. Background and daylight unchanged. Realistic hands and fingers, stable face identity, no morphing, no text.
```
