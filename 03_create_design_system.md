# Prompt 3: Create Design System (The Boss Move)

**Use with:** Claude Code, Cursor, Windsurf, or any AI coding assistant

**Purpose:** Generate a design concept and design system that locks in your visual language forever

---

## Why This Matters

After Prompt 2, your app looks good. But the next feature you add? The AI will
guess. Guesses on guesses degrade over time, and you'll drift back to generic.

This prompt creates two documents that solve that:

| Document | What It Is | What It Does |
|----------|------------|--------------|
| **Design Concept** | The "why" and "feel" | Guides decisions when the design system doesn't cover something |
| **Design System** | The exact specs | Tells the AI exactly what values to use for every component |

With these in place, every future feature follows the same visual language automatically.

---

## The Prompt

This is a longer prompt. Copy the entire block below:

````markdown
# Request

We want to codify the design of an application into a design system. This is a
creative process and needs to be done thoughtfully and creatively -- always
staying true to the design concepts and principles found in this current design.

To do this we will be creating a design concept and a design system. The design
concept will be used to guide the creation of the design system. The design system
will be used to create the application going forward.

There will be two main outputs from this process:
- a design concept
- a design system

# Design Concept

A design concept is a high-level description of the design of an application. It
is a collection of design principles and guidelines that are used to create a
design system. This is a document typically created by a creative director or
designer. It is a document that is used to guide the creation of a design system.

## Analyze Design

Deeply analyze the design of the current application to create a
design concept file in this project that describes the style and
design of every UI component needed in a design system at a high level, like a
creative director.

Capture high-level guidelines for:
- structure
- spacing
- fonts
- colors
- design style
- design principles

The goal with this file is to instruct AI to be able to replicate this look
easily in this project.

## Output
Output your design concept into the design concept file path from the output
file inputs at the end of this prompt.

# Design System

Use the design concept to guide the creation of the design system.

## Design a Design System

We are creating a DESIGN SYSTEM from the design found in this application. This
application does not have all components found in a design system. We need to
create a design system that includes many common components found in the
applications. This is a creative process and needs to be done thoughtfully and
creatively -- always staying true to the design concepts and principles found in
this current design.

## Intention
We want to outline the exact styling for all components and styles in this app,
along with high-level design guidelines, as there may be future components created
and it should be clear to the building agent how to create new styles for it.

## Output
Output your design system into the design system file path from the output
file inputs at the end of this prompt.

Output file inputs (edit only these lines):
- Design concept file path: docs/design_concept.json
- Design system file path: docs/design-system.json
````

---

## How to Use

1. Get your app looking the way you want (using Prompts 1 and 2)
2. Run this prompt in your AI coder
3. You'll get two files in `docs/`:
   - `design_concept.json` - The creative direction
   - `design-system.json` - The technical specs
4. For all future work, tell your AI: "Use the design system in `docs/design-system.json`"

---

## What You Get

**Design Concept** (example snippet):
```json
{
  "vision": "Create a dreamy, calming digital environment that feels like looking through frosted glass at a serene sky",
  "mood": {
    "emotions": ["calm", "playful", "airy"],
    "inspirations": ["soft clouds", "soap bubbles", "morning light"]
  },
  "principles": [
    "Breathing room over density",
    "Soft edges over sharp corners",
    "Subtle motion over static interfaces"
  ]
}
```

**Design System** (example snippet):
```json
{
  "colors": {
    "primary": "#6B9BD2",
    "surface": "#F8FAFC",
    "text": "#1E293B"
  },
  "borderRadius": {
    "sm": "8px",
    "md": "16px",
    "lg": "24px"
  },
  "shadows": {
    "card": "0 4px 12px rgba(0,0,0,0.08)"
  }
}
```

---

## Tips

- **Run this AFTER your app looks good** — it codifies what exists
- **The design concept is for edge cases** — when you need to make a decision the system doesn't cover
- **The design system is for implementation** — exact values, no guessing
- **Include both files in context** when building new features
- **Update these docs** if your design evolves significantly

---

## You're Done

With these two documents, your app will never drift back to generic. Every new
feature follows the same visual language. You're not just theming anymore—you're
designing.
