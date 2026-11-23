---
name: heymax-motion-guidelines
description: Use the HeyMax guidelines preview and Figma references to spec or QA HeyMax motion for campaigns and in-app UI. Use when turning a HeyMax brief into a motion treatment or checking a proposed animation against the brand.
---

# HeyMax motion guidelines

Use the guide to pick a HeyMax motion treatment and communicate it to a designer or engineer. The browser demos are references, not production assets. Stay in the medium requested: campaign motion can be more expressive; in-app motion should clarify what changed and keep the interface responsive.

## References

- [Official HeyMax brand guidelines](https://marketing.heymax.ai/design) and [Logo Toolkit](https://laurent-heymax.github.io/heymax-logo-toolkit/): published reference and files.

- [Brand guidelines · Start here](https://www.figma.com/design/osbBQgXRz6Rd19ZnuqMoWX/Design-System--external-?node-id=292-8748): official brand rules and navigation.
- [Logo usage](https://www.figma.com/design/osbBQgXRz6Rd19ZnuqMoWX/Design-System--external-?node-id=16-1788): use the prescribed lockup for the placement; the standalone M is reserved here for in-app motion and merch.
- [Product UI](https://www.figma.com/design/osbBQgXRz6Rd19ZnuqMoWX/Design-System--external-?node-id=18-1426) and [INFLIGHT components](https://www.figma.com/design/osbBQgXRz6Rd19ZnuqMoWX/Design-System--external-?node-id=163-8653): start here for an editable in-app surface.
- [Campaign master template](https://www.figma.com/design/osbBQgXRz6Rd19ZnuqMoWX/Design-System--external-?node-id=421-11264): reference examples for banner and social layouts, not an animation master.

## Open the preview

Open the [HeyMax motion guide](https://laurent-heymax.github.io/heymax-motion-preview/guide/#motion). For the interactive basics and easing values, jump to [Basic motion](https://laurent-heymax.github.io/heymax-motion-preview/guide/#motion-basics).

The browser studies are illustrations, not exportable production motion files. Use the official brand guide for approved logos and original motion assets.

To use this as an agent skill, keep it as `heymax-motion-guidelines/SKILL.md` in your agent’s project skills directory and ask it to use `heymax-motion-guidelines` for your brief. You can also hand it this Markdown file directly.

## Workflow

1. Identify the surface, audience, placement, and message. Use its approved Figma frame and copy. Keep logo geometry, clear space, and the template's text width and line limits; shorten the copy rather than squeezing it to fit.
2. Open **08 · Motion** in the browser guide and use **The lift** for a text reveal. Choose **Lines** for a short message that should read as one thought; choose **Words** when the order of emphasis matters. Preview at **1X** for the intended pacing and **1/2X** to inspect the sequencing. Half speed is a review aid, not a production timing recommendation. Do not recreate the removed character-by-character option.
3. For a campaign, show the treatment at the actual crop and hold the final copy and lockup long enough to read. For the app, name the trigger and the before/after states. Keep content and actions available while the animation runs; supply a reduced-motion treatment that preserves the same outcome without the lift.
4. Hand off the Figma frame, motion pattern, trigger or cue, duration/stagger/easing at **1X**, final hold or end state, and any reduced-motion behavior. Read the values from the current guide or implementation rather than measuring the slowed preview. Label any proposed departure from the guide as a proposal.

**The lift at 1X (25 fps reference):** enter over 24 frames with `cubic-bezier(.22, 1, .36, 1)`; stagger lines by 4 frames or words by 2. The demo holds for 1,400 ms, then exits over 12 frames with `cubic-bezier(.11, 0, .5, 0)` and a 1-frame stagger. Use these as a starting point for the lift, not as defaults for unrelated UI transitions.
