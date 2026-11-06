# Golden prompt: Ellie (Model D)

> Do not edit without Lucas's explicit approval (SKILL.md, rule 5).

## A. Origin job record, verbatim

Copied character for character from the Higgsfield job record, read on 25 Oct 2026 through the Higgsfield connector. Confirmed the same day by a side-by-side visual check: this result is the image saved in the AmeriVita-Model-D Element (media_input `0198679e-0c40-4b5c-b1a9-d5b7eed88406`), unedited.

- **job_id:** `1d3f407b-3604-459f-9fc2-ad46c4ef6f04`
- **date:** `createdAt` 1792159586.039997 = 2026-10-16 14:06:26 UTC (15:06 UK time)
- **model id:** `text2image_soul_v2`
- **status:** `completed`
- **prompt:**

```
Casting test portrait, authentic UK editorial lifestyle photograph shot on Sony A7 IV, 50mm lens. A naturally attractive British woman, 31 years old, medium-length chestnut brown hair with subtle natural waves, hazel-brown eyes, softly defined cheekbones, natural lips, understated make-up, visible skin pores, very subtle freckles, realistic under-eye texture, slight natural facial asymmetry, relaxed genuine half-smile. Cream knit jumper. Standing by a window in a lived-in British home with cream walls and natural wooden furniture, soft overcast daylight from the window, realistic shadows, shallow depth of field, natural colour grading, no retouching, no text.
```

- **params (verbatim):**

```json
{
  "width": 1536,
  "height": 2048,
  "batch_size": 1,
  "seed": 907391,
  "enhance_prompt": false,
  "use_sage_attention": false,
  "quality": "1080p",
  "use_relax": false,
  "style_id": "3db34ab5-3439-4317-9e03-08dc30852e69",
  "style": {
    "id": "3db34ab5-3439-4317-9e03-08dc30852e69",
    "name": "General",
    "url": "https://cdn.higgsfield.ai/soul-v2-style/f33d85f2-6521-4fa8-8e8f-894cfbdee578.webp",
    "strength": null
  },
  "style_strength": null
}
```

- **aspect ratio / duration / resolution fields:** not present in the record (size is width 1536 × height 2048; quality "1080p")
- **media inputs:** none (no `medias` field in the record)
- **reference_id / soul_id:** not present in the record (text-to-image, no trained Soul)
- **result_url:** https://d8j0ntlcm91z4.cloudfront.net/user_3CiE0dpc5yRHLrqtZoz7h6B2IQN/hf_20261016_140626_1d3f407b-3604-459f-9fc2-ad46c4ef6f04.png
- **preview (min) url:** https://d8j0ntlcm91z4.cloudfront.net/user_3CiE0dpc5yRHLrqtZoz7h6B2IQN/hf_20261016_140626_1d3f407b-3604-459f-9fc2-ad46c4ef6f04_min.webp

Re-running section A exactly (same model, prompt, seed and params) is the way to recreate the master portrait itself. It is **not** the way to make new scenes: Soul V2 text-to-image with a new prompt produces a different woman.

## B. Locked production setup (approved 25 Oct 2026; not part of the verbatim record)

Use this for every new shot. It is what kept her face consistent across about 35 stills and 6 videos.

- **reference_id (Element, default):** `e9783c1f-0669-4d38-b14c-df17b3403e07` (AmeriVita-Model-D-v2: master portrait + three-quarter left, profile, three-quarter right, laughing, mid-sentence)
- **reference_id (Element, master record / fallback):** `7811391d-526a-4bd2-a6ab-d02aab51c43a` (AmeriVita-Model-D, master portrait only)
- **hero still:** job `1d3f407b-3604-459f-9fc2-ad46c4ef6f04` (see `hero-still.md`)
- **still model:** `nano_banana_2`, resolution `2k`, aspect `4:5` (feed) or `9:16` (Reels/Stories); for edits, pass the approved frame as the image reference
- **video model:** `kling3_0`, mode `pro`, cfg_scale `0.5`, sound `off`, aspect `9:16`, duration 3-5 s, `start_image` = an approved still. Talking clips: Higgsfield `ugc-video` workflow (`seedance_2_5`, omni_reference)
- **identity-lock block (paste word for word at the start of every prompt):**

```
<<<e9783c1f-0669-4d38-b14c-df17b3403e07>>> (same face, freckles and wavy chestnut hair with caramel ends exactly), a British woman around 31, shoulder-length wavy chestnut hair with lighter caramel ends and a side parting, hazel-green eyes, clearly visible freckles across her nose and cheeks, softly defined cheekbones, natural lips, slight natural facial asymmetry, visible skin pores, understated make-up.
```

Why the block differs from the section A prompt: the master image shows hazel-green eyes and clearly visible freckles, not "hazel-brown" and "very subtle". The block follows the image so the text never fights the reference.
