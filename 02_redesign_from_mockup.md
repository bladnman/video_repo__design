# Prompt 2: Redesign from Mockup

**Use with:** Claude Code, Cursor, Windsurf, or any AI coding assistant

**Purpose:** Apply the visual style from your mockup image to your actual application code

---

## What This Does

You give it the mockup image from Prompt 1. It redesigns your app's code to match
that visual style—colors, spacing, typography, component styling—while keeping all
your functionality intact.

---

## The Prompt

```
Use the visual reference described at the end of this prompt as the basis for a UI redesign.

Redesign the application's visual style, layout, spacing, and component expression
to match the theme and design language shown in the image.

Important constraints:
- Preserve the application's existing structure, hierarchy, and functionality—how
  the app works should remain the same
- Focus on UI and interaction design, not new features or workflows
- Any imagery, illustrations, photos, or complex visual assets in the screenshot
  may be approximated, simplified, or ignored if source assets are unavailable

The goal is to re-theme the application as closely as possible to the provided
design using realistic, buildable UI components, while maintaining usability and
clarity.

Visual reference:
(Attach your image, link, file path, or description below)
- Reference details: 

```

---

## How to Use

1. Copy the mockup image from Prompt 1
2. Provide the visual reference to your AI coder (attach, link, or describe)
3. Fill in the `Visual reference` lines at the bottom of the prompt
4. Let it restyle your app

---

## What It Does Well

- Pulls color schemes from the image
- Matches spacing and padding patterns
- Applies rounded corners, shadows, visual weight
- Updates typography feel

## What It Won't Do

- Recreate complex illustrations or graphics (it will simplify or skip them)
- Match fonts exactly (it approximates)
- Add new features

---

## Tips

- **Just one component?** Tell it: "Only redesign the header" or "Focus on the card components"
- **Not pulling enough?** Be specific: "Use the exact color palette from this image"
- **Adding too much?** Add: "Keep it simple—no decorative elements"
- **First pass not perfect?** That's normal. Push in on the details that matter:
  "Make the buttons more rounded" or "The shadows should be softer"

---

## Next Step

Once your app looks the way you want, go to **[Prompt 3: Create Design
System](03_create_design_system.md)** to lock it in forever.
