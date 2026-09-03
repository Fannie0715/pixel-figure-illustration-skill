---
name: pixel-figure-illustration-skill
description: Turn Chinese articles, notes, scripts, product stories, and AI topics into 3:4 Xiaohongshu narrative illustrations with a consistent user-provided character, accurate layered Chinese text, and 2-Part, 3-Part, or 4-Part pacing. Use for 像素小人配图、小红书手绘内容图、漫画叙事图文、文章拆图, or switching between black-ink and denim-blue line-art variants.
---

# Pixel Figure Illustration

Create a sequence of hand-drawn narrative content images, not an infographic. Each page should feel like a person is telling a story while sketching the important moments.

## Non-negotiable rules

1. One page communicates one core idea. Add a page instead of crowding or shrinking text.
2. Use [assets/ip-reference/canonical-ip.png](assets/ip-reference/canonical-ip.png) as the canonical character reference. Change pose, expression, viewpoint, props, and scene; preserve the face, hair, silhouette, proportions, youthful hand-drawn feeling, and identifying details. Change the drawing treatment, not the person.
3. Text and illustration form one asymmetrical composition. Reject PPT, knowledge-card, fixed left-text/right-image, equal columns, panels, UI cards, and decorative borders.
4. Prefer actions, relationships, and real scenes over icons or literal diagrams. Use one main scene and at most one supporting scene.
5. Keep a pure white background and roughly 35–50% breathing room.
6. Default to a 3:4 canvas (1242 × 1660 or an equivalent high-resolution size).

## Visual styles

### Black Ink + Soft Accent Color

- Pure white background, black text, and loose black hand-drawn linework.
- Allow one or two low-saturation accents, such as pale yellow, blue, pink, green, or purple.
- Accent colors should cover no more than about 15–20% of the image. They emphasize or distinguish; they must not turn the page into a full-color illustration.
- Small areas of gray shading or dot texture are acceptable. Avoid gradients, glossy lighting, 3D, large color fields, and polished vector-art finishes.

### Denim Blue Line Art

- Pure white background with one primary deep denim-blue ink color.
- Use blue contours, sparse hatching, and occasional small solid-blue areas while keeping abundant white space.
- “Denim” describes the ink color and tactile drawing language. It is not a Western theme.
- Reject cowboy hats, horses, deserts, cacti, saloons, sheriff imagery, brown palettes, beige vintage paper, and distressed Western-poster styling.

## Page pacing

Honor an explicit user choice. Otherwise select by content and prefer 3-Part.

| Mode | Use when | Text per part | Total text | Visual rhythm |
|---|---|---:|---:|---|
| 2-Part | A sharp idea, contrast, turn, opening, or closing | 15–30 Chinese characters | 35–60 | Largest art, loosest page |
| 3-Part | A normal narrative: start → change → result | 12–25 | 40–70 | Default |
| 4-Part | Four genuinely sequential beats or compact steps | 8–20 | 45–75 | Fastest rhythm |

Treat parts as narrative beats, never as equal rectangular panels. Beats may interleave and occupy unequal space. Aim to stay below 90 Chinese characters on every page. When the copy exceeds the selected range, split it into another page instead of reducing type size.

## Content workflow

1. Understand the source and identify the single narrative spine.
2. Break it into page beats. For each page, write the one idea the reader should remember.
3. Select 2-Part, 3-Part, or 4-Part pacing for each page.
4. Rewrite lightly for image reading: remove repetition, shorten sentences, reorder for clarity, and use natural spoken phrasing without changing the user's position.
5. Define a character action and scene for each beat. Illustrations should perform the moment, not repeat the nouns as icons.
6. Alternate page rhythms across a carousel. Do not reuse the same composition on every page.
7. Generate illustration layers without long body copy, then typeset the exact Chinese text separately in HTML, SVG, Canvas, or another deterministic layout system.
8. Export all pages at the same dimensions and run the QA checklist.

## Typography and layout

- Usually use 2–4 text blocks, each about 1–3 lines.
- Establish a clear hierarchy: one large narrative sentence, medium supporting lines, and small annotations only when necessary.
- Do not require a title on every page. Do not add automatic page numbers, section labels, or bullets.
- Use bullets only when the source is truly a checklist or instructional sequence.
- Let text and character placement respond to each other. Use off-center balance and meaningful empty space.
- Do not ask an image model to render long Chinese passages. Keep final text editable and exact.

## Deliverables

Before rendering, provide or internally establish a page plan with: page beat, exact copy, part mode, character action, scene, text placement, and selected visual style. Final output should include editable layout source when the environment supports it, plus high-resolution PNG exports.

## QA checklist

Reject or revise a page when any answer is no:

- Is the page faithful to the source and limited to one memorable idea?
- Does the character still match the canonical IP in face, hair, silhouette, proportions, and identifying details?
- Is the selected part count a narrative rhythm rather than a grid?
- Is the copy within the selected range and below about 90 Chinese characters?
- Is all Chinese text accurate, readable, and typeset outside the image-generation layer?
- Does the page avoid PPT structure, cards, fixed columns, default numbering, and unnecessary bullets?
- Are there no more than two main scenes, with actions or relationships preferred over icons?
- Is there ample white space and a pure white background?
- For Black Ink, are there at most two soft accent colors covering no more than 15–20%?
- For Denim Blue, is the page free of brown, beige paper, cowboy hats, horses, deserts, cacti, and other Western imagery?
