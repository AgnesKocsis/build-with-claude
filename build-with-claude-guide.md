# Build With Claude
## A Divi 5 AI Workflow

*A practical guide for Divi 5 web designers*

**For:** Divi 5 web designers, any niche
**Includes:** Skill files + starter prompts
**Prerequisite:** Basic Divi 5 knowledge
**Credit:** Shashank Gupta · divilove.com

---

## Chapter 1: Claude is the builder. You are the interior designer.

Before we get into any of the how, let's talk about what this actually is — and what it isn't.

When I first started using Claude for Divi work, I had the same quiet worry a lot of designers have: is this going to replace me?

After building a full six-page website template system with it, I can tell you: no. But understanding why not changed how I think about AI tools entirely.

> "Claude builds the house. You get to decorate it."

Think about how a building project actually works. The builder puts up the structure — the walls, the floors, the plumbing, the wiring. All the technical precision work that has to be exactly right or nothing functions. But the builder doesn't choose the wallpaper. They don't decide which rooms feel warm and which feel quiet. They don't know what your client needs to feel when they walk through the front door.

That's the interior designer's work. And no builder can do it for them.

Working with Claude in Divi is exactly like this. Claude handles the structural work that's time-consuming, repetitive, and technically demanding: generating valid JSON, keeping your design tokens consistent across every page, catching mismatched tags before they silently break a layout. It does this without getting tired, without drifting, without forgetting that your button border-radius was 8px on the homepage.

But Claude doesn't know your client. It doesn't know the feeling they want their visitors to have. It doesn't know how to make a page feel like it was made for one specific person.

You do. That's your skill and it is not replicable.

### What changes when you work this way

What actually changes is where your time goes. Right now, a meaningful chunk of your design hours probably goes into things like: hunting down which hex value you used on that card background three pages ago, rebuilding a section because the JSON broke and you can't figure out why, making the same spacing decision twelve times on twelve different pages.

When Claude handles the structural work, those hours go somewhere else. You spend more time on the decisions that actually require you — the ones that make a website feel considered rather than assembled.

> **In practice, this means:** Claude generates consistent, validated Divi 5 JSON from your design tokens. You decide what the tokens are, what the pages need to communicate, and whether the result feels right. You're not removed from the process — you move to the part of it that only you can do.

### How this workflow came together

It started with a set of skill files from Shashank Gupta at divilove.com — structured knowledge documents that teach Claude the confirmed, tested JSON schemas for every Divi 5 module type. Before having them, Claude's Divi output looked plausible but broke on import. After uploading the skill files, Claude generated valid JSON correctly.

That was the first piece. Claude could now build. But I didn't yet know what to ask it to build.

**Shashank Gupta's skill files at divilove.com**
The technical foundation. Structured knowledge documents that teach Claude valid Divi 5 JSON schemas — module types, nesting rules, attribute names, and the common mistakes that silently break layouts.

**Ania Romańska's work at divilover.com**
The conceptual framework. Understanding what a Divi 5 design system actually is — global colour tokens, number variables, fluid type scales with clamp(), presets — and why you build the system before you build any pages.

**Feeding Claude real Divi 5 exports**
The skill files teach Claude the schemas in theory. To sharpen that further, I uploaded real finished Divi 5 page exports directly into the Project — actual JSON from working pages. Claude could now cross-reference theory with real examples, which improved the accuracy and confidence of everything it generated.

**The key insight: design system first, pages second**
Instead of jumping straight to page templates, first use Claude to build the design system itself — all global colours, variables, and presets — and get that imported into Divi before writing a single content page. Every page then draws from the same source of truth automatically.

**The Blueprint system**
Applying the full workflow to a real project — six complete Divi 5 page templates, all drawing from a shared design system, with a Python build pipeline and validated JSON. Proof that the approach works at scale — and the foundation for a starter website I can reuse across my entire niche.

This guide documents that workflow so you can apply it to your own projects — whatever niche you design for. You bring the design decisions, the client understanding, and the creative direction. Claude handles the structure.

---

## Chapter 2: How Claude learns what it needs to know

Claude doesn't know your workflow, your niche, or Divi 5's specific JSON format by default. Claude Projects and skill files are how you fix that — once, persistently.

### What is a Claude Project?

A Claude Project is a persistent workspace in your Claude account. Files you upload to a Project stay available for every conversation within it — Claude draws on them without you having to paste or re-explain anything. It's the difference between briefing a contractor from scratch every session and having a colleague who already knows the project.

For Divi 5 work, a Project lets you upload your skill files once and have Claude apply that knowledge to every page you build together, throughout the entire project.

### What are skill files?

Skill files are structured knowledge documents — written in a format Claude knows how to read and apply. The skill files included with this guide are built on the technical foundation created by Shashank Gupta at divilove.com. They contain the confirmed JSON schemas for Divi 5 modules, the nesting rules, the styling properties, and the common mistakes. When these are in your Project, Claude generates valid Divi 5 JSON rather than guessing.

> **Credit where it's due:** The technical Divi 5 knowledge that makes this workflow possible was originally pioneered by Shashank Gupta at divilove.com — his work on Divi 5 JSON schemas is what made this whole approach possible. The skill files included in this bundle are built on that foundation and refined through real project work. The conceptual understanding of Divi 5's design system comes from Ania Romańska at divilover.com. Her course on Divi 5 design systems is something I genuinely recommend taking before or alongside this guide.

### The skill files in this bundle

| File | What it teaches Claude |
|------|------------------------|
| `01-divi5-base.md` | Core rules, nesting hierarchy, validation checklist. Always required. |
| `02-divi5-layout.md` | Section, row, column, group structure and the flexbox system. |
| `03-divi5-styling.md` | Background, spacing, border, typography, sizing, and token references. |
| `04-divi5-modules-content.md` | Heading, text, button, image, blurb, CTA, testimonial, and more. |
| `05-divi5-modules-interactive.md` | Accordion, toggle, tabs, contact form, and the interaction system. |
| `06-divi5-patterns.md` | Real-world layout patterns — hero, features, CTA, testimonials. |
| `07-divi5-design-system.md` | The complete design system workflow — colours, variables, presets. |

### Setting up your Claude Project

**Step 1 — Create a new Project**
In Claude.ai, open the Projects section and create a new project. Name it for the client or site you're building — this becomes your persistent workspace for that project.

**Step 2 — Upload the skill files**
In the Project settings, upload all the skill files from this bundle. Claude indexes them immediately. You don't need to reference them by name in your prompts — Claude knows they're there.

**Step 3 — Test it's working**
Start a conversation and ask: *"What are the non-negotiable rules for Divi 5 JSON generation?"* Claude should answer from the skill files clearly and specifically. If it does, you're set up correctly.

**Step 4 — Add your design system once it's built**
After Chapter 3, you'll have a design system JSON file — one file containing your global colours, number variables, and presets. Upload that to the Project too — Claude will then have your specific tokens available in every conversation without you pasting them each time.

**Step 5 — Upload real Divi 5 exports to sharpen Claude's output**
This one made a meaningful difference: export finished Divi 5 pages from your own site or client projects and upload the JSON files to the Project. The skill files give Claude the theory — real exports give it working examples to cross-reference. Claude's generated JSON becomes noticeably more accurate and confident when it has both.

---

## Chapter 3: Design system first — always

Before any page, before any section, before any module — build the design system. This is where most of the design thinking happens, and it's where you do your most valuable work.

The instinct is to jump straight to pages. But every time you build a page without a design system, you're making design decisions that should have been made once and reused — on the fly, under time pressure. The result is a site that works but drifts: slightly different button colours, inconsistent section padding, heading sizes that don't quite match across pages.

The design system is where you make those decisions once, deliberately, with space to think. Then every page just uses them.

> **Recommended resource:** Ania Romańska at divilover.com teaches a course specifically on Divi 5 design systems — how global variables work inside the builder, how presets are structured, the full token architecture. I'd genuinely recommend taking it alongside this guide. Her blog is also an excellent free resource, including her article *"What Is a Design System (and How It Works in Divi 5)"*. Understanding both sides — the UI and the JSON we generate with Claude — is what makes the whole workflow click.

### What your design system needs to define

**Colour tokens**

Named colour variables, each with a defined role — not just a name. Don't just call something "Green." Call it "Accent" and define what it's for. Primary buttons only? Also icon colours and active states? Deciding upfront prevents the drift where you end up with six slightly different versions of the same colour across a site.

Important: don't ask Claude to choose your colours for you. Colours are a design decision — they carry the emotional weight of the brand, and that's your job. Instead, build a moodboard first. Pull together images, colour swatches, references — anything that captures the feeling you're designing for. Then bring that to Claude: *"Here is my moodboard and these are the colours I'm working with. Help me define them as a token system with named roles."* Claude organises and structures what you've already decided. You stay in creative control.

A good palette for a service-based site typically needs: one accent colour (and a soft/muted version), three ink shades (dark, medium, light) for text hierarchy, three background shades (page, surface, alternate), and a border colour. Ten tokens covers most situations.

**Spacing tokens**

Fixed rem values for padding and margins. A simple scale covers almost everything: `1rem / 1.5rem / 2rem / 3rem / 4rem / 6rem`. One important Divi 5 constraint: `clamp()` fluid values work for font sizes but Divi silently drops them from spacing fields. Keep spacing as fixed values.

**Typography**

Same principle as colours — choose your fonts before you open Claude, not the other way around. Find a site whose typography you love. It might be a competitor, a brand in a completely different industry, a design portfolio — doesn't matter. Screenshot it, note the font pairing, describe what it feels like. Then bring that reference to Claude: *"I love the type feel on this site — it uses [serif] for headings and [sans] for body. Can you build me a fluid type scale using these two fonts with clamp() values for Divi 5?"*

That's exactly how the type scale in this workflow was developed — I found a site whose typography felt right, shared it, and we built the scale from that reference rather than from abstract numbers. The result felt intentional because it was.

Use `clamp()` values for font sizes so they scale fluidly between mobile and desktop with no breakpoint tweaking. In Divi 5, font families are stored as global content variables, so changing your site's font means changing one value and watching everything update.

**Module presets**

Saved style configurations for sections, rows, columns, and the modules you use most. Presets carry your visual identity — a "default section" preset means you never have to style the same thing twice across twenty pages.

### Building your design system with Claude

The starting point is always your moodboard — not a prompt. Before you open Claude, gather your references: colours you've chosen or pulled from a brand brief, fonts you love, websites whose typography or overall feel you want to reference. Claude's job is to take those decisions and structure them into a token system, not to make the creative decisions for you.

> *I've put together a moodboard for this project. The colours I'm working with are [list your hex values or describe them from your moodboard]. The font pairing I want is [heading font] for headings and [body font] for body — I love how [name a site or describe the feel] handles its typography. Can you organise these into a named token system with a defined role for each colour, and build me a fluid type scale using clamp() values?*

> *Good. Now generate the design system JSON file — the single file that contains global_colors, global_variables, presets, and all the other required keys. Use the correct format from the skill files. I'll import this into Divi before building any pages.*

Review the output. Adjust what doesn't feel right. Import the design system JSON file into Divi before you touch a single page — it's one file containing your global colours, number variables, and presets all together. This is your foundation — everything else rests on it.

> "You change one token. Every element using it updates everywhere. That's what a system actually means."

---

## Chapter 4: Building pages — the six-stage workflow

With your design system in place, every page Claude generates will be consistent — the same colours, the same spacing, the same presets, automatically. Honestly, the first time it works end-to-end it feels like magic. Claude handles the structural precision work, and you get to focus on what you actually love: design.

Every page follows the same six stages. The workflow exists because skipping stages always costs more time than following them.

**Stage 1 — Define the page's job**
One or two sentences: what is this page for, what should a visitor feel, and what's the one thing they should do by the time they leave. This is your brief. Write it down before any design work starts — it makes every subsequent decision easier.

**Stage 2 — HTML review first**
Ask Claude to produce a self-contained HTML file showing the full page: your design system colours and fonts, placeholder images with correct proportions, and real placeholder copy written in your client's voice. This is your design review stage. You see the page before any JSON is written.

**Stage 3 — Refine copy and layout**
Work through the HTML section by section. Headlines, body text, button labels, section order. The copy and layout need to be right at this stage — changing them after JSON generation means rebuilding. This is where the design thinking happens.

**Stage 4 — Approve the HTML**
When the page looks and reads right, you give Claude the go-ahead to generate JSON. Not before. The HTML review is your checkpoint — it exists to catch layout and copy decisions before they're baked into markup that takes longer to change.

**Stage 5 — Generate, validate, import**
Claude generates the Divi 5 JSON using the skill file schemas and your design system tokens. Validation checks run before the file is written. Import into Divi via Library → Import & Export → Import. Tick "Import Presets" for the design system import only. All subsequent page imports do not need this ticked — the presets are already registered in Divi globally after the first import.

**Stage 6 — Make it yours**
This is where the interior designer takes over. Replace placeholder images with your real photography, graphics, custom icons, and patterns. Swap placeholder copy for your client's actual words. Fine-tune spacing, adjust anything that doesn't feel quite right, and add the personal touches that make the site feel like it was made for one specific person. Claude built the house — now you decorate it.

*This step is entirely yours. No AI can do it for you.*

> **Why the HTML review step is not optional:** The HTML file isn't extra work — it's the step that saves you from the import → look wrong → debug → fix → reimport loop. When you approve the design in HTML first, the JSON import almost always works correctly the first time. Skip it and you're doing twice the work.

### What to say at each stage

> *I'm building a [page type] for [client description]. The page's job is to make someone feel [feeling] and understand [what the business does]. The main action is [CTA]. Using our design system, build me an HTML review file — don't generate any JSON yet. I want to see and approve the layout and copy first.*

> *The hero headline feels too [generic / salesy / flat]. The client works with [audience]. Give me five alternatives that feel more [specific direction] — not a promise of transformation, just honest and direct.*

> *The HTML is approved. Now generate the Divi 5 JSON for this page. Use our design system tokens throughout, follow the module schemas from the skill files, and run all validation checks before writing the output file.*

---

## Chapter 5: Starter prompts — copy and use immediately

These are the exact prompts to start working. Adapt the parts in brackets to your project.

### Testing your project setup

> *What do you know about Divi 5 JSON generation from the skill files? Specifically: what are the non-negotiable structural rules, and what are the most common mistakes that silently break a layout?*

### Starting a new design system

> *I've built a moodboard for this project. My colours are [list your hex values — don't ask Claude to choose them]. The fonts I want are [heading font] and [body font] — the typography feel I'm going for is similar to [reference site or description]. Can you organise these into a named token system with defined roles, and build me a fluid type scale using clamp() values for Divi 5? Show me the output before generating any JSON.*

### Generating design system JSON

> *Here's the approved design system: [paste your tokens, type scale, spacing values]. Generate the design system JSON file — one single file containing global_colors, global_variables, presets, and all required keys, in the correct Divi 5 format from the skill files. I'll import this into Divi before building any pages.*

### Starting a new page

> *I need to build a [page type] for this project. Its job is to [what the page must do]. The visitor should feel [feeling] and the main action is [CTA]. Using our design system, build me an HTML review file first — full page, real placeholder copy, correct colours and fonts. No JSON yet. I want to approve the design before we build anything.*

### When the copy isn't landing

> *The [section name] copy feels too [generic / salesy / abstract / stiff]. The audience is [describe them — who they are, what they're struggling with, what they want to feel when they find this site]. Write five alternative versions that feel more [honest / direct / warm / specific to this person]. Not a formula. Not a template. Something that reads like it was written for one person.*

### Generating page JSON

> *The HTML is approved. Generate the Divi 5 JSON for this page. Use our design system tokens throughout — no hardcoded hex values. Reference the module schemas from the skill files for every module type. Run the structural validation checks before writing the output file and tell me the results.*

### Debugging after import

> *After importing this page into Divi, [describe exactly what looks wrong — which section, which element, what it's doing versus what it should do]. Here's the relevant part of the JSON: [paste the section]. Can you identify what's causing it and generate a corrected version?*

---

## Chapter 6: Where to go from here

You have the workflow, the skill files, and the prompts. Here's how to build on it over time.

### Go deeper on Divi 5

**Divi Lover · Ania Romańska**
The best Divi 5 resource available, and the one that shaped how I think about design systems. Ania runs a course specifically on Divi 5 design systems — it's not always open for enrolment, but it's worth checking and getting on the waitlist. Her blog at divilover.com is also consistently excellent. Check her courses at divistylistacademy.com.

**Divi Love · Shashank Gupta**
The technical groundwork this whole workflow rests on. Shashank's research into Divi 5's JSON schemas is what made Claude-assisted Divi development possible in the first place. Worth knowing about and crediting: divilove.com.

### Build your own pattern library

Every time you build a section that works well — a services grid, a testimonial layout, a pricing block — save the JSON as a pattern. Over time you build a library of tested, validated components you assemble quickly rather than generate from scratch. The workflow compounds: each project makes the next one faster.

### Extend the skill files

The skills included here cover the core modules. As you work with specific modules more — sliders, data modules, interactive elements — you can build additional skill files that document the patterns you use most. A skill file is just a structured markdown document. The more specific it is to your workflow, the more directly useful it becomes.

### Apply it to any niche

This workflow transfers to any service-based website, any industry, any client type. The design system approach, the six-stage workflow, the validation pattern — none of it is niche-specific. What changes is the colour palette, the tone of the copy, the structure of the pages. Those are your creative decisions. The system handles everything else.

If you work with a specific niche, you can build a starter website with Claude once and reuse it across every client — same system, different content. Make this workflow yours. My own starter template for healers and coaches is at [blueprint.soulmagicstudio.com](https://blueprint.soulmagicstudio.com) if you want to see what a finished example looks like. This is a new workflow and I'm still learning as I go — if you discover something that could make it better, I'd genuinely love to hear it.

---

## Quick Start — Step by step checklist

Ready to start? Here's the full process at a glance.

### Step 1 — Set up your Claude Project

- [ ] Create a new Project in Claude.ai
- [ ] Upload all 7 skill files
- [ ] Test: ask *"What are the non-negotiable rules for Divi 5 JSON generation?"*

### Step 2 — Build your design system

- [ ] Put together your moodboard — colours, fonts, reference sites
- [ ] Ask Claude to define your colour tokens and type scale from your moodboard
- [ ] Ask Claude to generate the design system JSON file
- [ ] Import into Divi: Library → Import & Export → Import → tick **"Import Presets"** (use a fresh Divi install — a local install works fine)
- [ ] Create a new page in Divi and insert the layout. Make any additional variables or presets you might need for the project
- [ ] Upload the tweaked design system JSON to your Claude Project

> ⚠️ **Only tick "Import Presets" once** — when importing the design system. All page imports afterwards do not need presets ticked. The presets are already registered in Divi from the first import. Ticking it again on page imports can overwrite your system.

### Step 3 — Build each page (repeat for every page)

- [ ] Define the page's job in one sentence
- [ ] Ask Claude for an HTML review file — no JSON yet
- [ ] Refine copy and layout in the HTML
- [ ] Approve the HTML
- [ ] Ask Claude to generate the Divi 5 JSON
- [ ] Import into Divi — **do not tick "Import Presets"**
- [ ] Add your real images, graphics, icons, and copy
- [ ] Fine-tune until it feels right

---

*Claude builds. You design. That's the whole idea. The structural work is handled. The creative work — the part that makes a website feel made for one specific person — that's still yours. It always will be.*

Figured out by Soul Magic Studio · soulmagicstudio.com
