# UI 设计参考库

> 精选自 [Refero Styles](https://styles.refero.design/)（styles.refero.design）—— 一个面向 AI 编码工具的高质量 `DESIGN.md` 设计系统库。本文档收录了与 **App/网站开发、人工智能产品、高级科技感、SaaS** 四类主题相关的 11 套设计系统全文，供团队在做 UI 设计 / 前端开发时直接参考或喂给 AI 编码工具（Cursor、Claude Code、v0、Lovable 等）作为风格上下文。

- 来源站点：https://styles.refero.design/
- 整理时间：2026-08-31
- 收录数量：11 套（可按需增补，见文末「如何更新」）

## 目录

### 🚀 SaaS 产品
1. [Linear](#linear--style-reference) — 午夜精密仪器风，暗色 SaaS 标杆
2. [Slack](#slack--style-reference) — 紫黑舞台，几何大字标题
3. [Calendly.com](#calendarcom--style-reference) — 藏青底色 + 冷石白，编辑感排期工具
4. [Atlassian](#atlassian--style-reference) — 白底企业蓝 + 撕纸边彩色装饰

### 🤖 人工智能
5. [Generative AI (fal)](#generative-ai--style-reference) — 白底像素风，开发者友好的生成式媒体平台
6. [Leonardo.ai](#leonardoai--style-reference) — 黑底巨幅紫色字标，AI 生图画廊
7. [Morphic](#morphic--style-reference) — 纯黑电影感画布，单一电光蓝强调色

### ✨ 高级 / 科技感
8. [Apple](#apple--style-reference) — 近白留白 + 单一蓝色，极致克制
9. [Superhuman](#superhuman--style-reference) — 暖调编辑感 + 酒红色，高端邮件工具

### 📱 App / 网站开发
10. [WhatsApp.com](#whatsappcom--style-reference) — 奶油底色 + 绿色行动色，温暖对话感
11. [Mobbin](#mobbin--style-reference) — 纯灰阶排版，App 截图画廊

---

# Linear — Style Reference
> midnight precision instrument

**Theme:** dark

Linear's design system is a midnight command center built on near-black surfaces (#08090a) with paper-white type and one electric acid-lime accent (#e4f222) that functions as a functional flashlight — small, high-contrast, and used sparingly to signal action. The interface treats darkness as a substrate rather than a theme: text is crisp white at tight tracking (-0.022em), weights sit in a low 400–510 band rather than bold, and borders are hairline-thin (0.5px) to let geometry do the work that shadows usually would. Components feel precision-machined — 6px and 12px radii, compact 8–12px paddings, and almost no decorative ornament — letting the product UI (issue cards, kanban boards, AI agent panels) be the only visual texture in an otherwise quiet system.

## Tokens — Colors

| Name | Value | Token | Role |
|------|-------|-------|------|
| Void | `#08090a` | `--color-void` | Page canvas, full-bleed backgrounds — the default everything sits on |
| Carbon | `#0f1011` | `--color-carbon` | Card surfaces, nav bars — one step above canvas for contained content |
| Obsidian | `#161718` | `--color-obsidian` | Elevated surfaces, deeper card panels |
| Graphite | `#23252a` | `--color-graphite` | Subtle borders, dividers, ghost button outlines — low-contrast structural edges |
| Smoke | `#383b3f` | `--color-smoke` | Hairline borders at higher contrast than graphite — section separators |
| Ash | `#62666d` | `--color-ash` | Muted body text, inactive icons, secondary metadata |
| Fog | `#8a8f98` | `--color-fog` | Tertiary text, placeholder copy, icon fills |
| Mist | `#d0d6e0` | `--color-mist` | Secondary headings, button text on dark surfaces |
| Bone | `#e5e5e6` | `--color-bone` | Near-white surface fills, high-contrast button text |
| Paper | `#ffffff` | `--color-paper` | Primary headings, hero type, max-contrast emphasis text |
| Acid Lime | `#e4f222` | `--color-acid-lime` | Primary action buttons, active nav indicators — electric accent that breaks the monochrome system |
| Pulse Green | `#27a644` | `--color-pulse-green` | Green outline accent for tags, dividers, and focused UI edges |
| Coral Red | `#eb5757` | `--color-coral-red` | Red wash for highlight backgrounds, decorative bands, and soft emphasis |
| Signal Teal | `#02b8cc` | `--color-signal-teal` | Decorative accent, informational icon fills |
| Iris Violet | `#6366f1` | `--color-iris-violet` | Tag/badge fills — soft chromatic punctuation on tags and labels |
| Lavender | `#8b5cf6` | `--color-lavender` | Secondary tag fills, category indicators |

## Tokens — Typography

**Inter Variable** — Primary UI and heading typeface. Substitute: Inter (variable) / system-ui. Weights 300/400/510/590. Sizes 10–72px. Letter-spacing -0.022em at 48–72px down to -0.010em at 13–16px. OpenType: `cv01, ss03, zero` on.

**Berkeley Mono** — Code-adjacent UI text (issue IDs like ENG-2703, keyboard shortcuts). Substitute: JetBrains Mono / IBM Plex Mono. Weight 400, sizes 12/14px.

| Role | Size | Line Height | Letter Spacing |
|------|------|-------------|----------------|
| caption | 13px | 1.2 | — |
| body-sm | 15px | 1.6 | -0.165px |
| body-lg | 20px | 1.33 | -0.24px |
| subheading | 24px | 1.33 | -0.288px |
| heading-sm | 32px | 1.13 | -0.704px |
| heading | 48px | 1 | -1.056px |
| heading-lg | 64px | 1 | -1.408px |
| display | 72px | 1 | -1.584px |

## Spacing & Shape

Base unit 4px · density compact. Spacing scale: 4/8/12/16/20/24/28/32/36/40/48/56/64/80/96/128px.

Border radius: cards 12px · pills 9999px · small 2px · badges 4px · inputs 6px · buttons 6px.

Layout: max-width 1200px · section gap 96px · card padding 24px · element gap 8px.

## Components

- **Primary Action Button (Acid Lime):** bg `#e4f222`, text `#08090a`, radius 6px, padding 10px 16px, Inter 14px/510. The one chromatic button in the system.
- **Nav Text Button:** transparent, text `#d0d6e0`, 13px/400, underline on hover.
- **Pill Button:** `rgba(255,255,255,0.05)` bg, text `#d0d6e0`, radius 9999px, 12–13px/400.
- **Ghost / Outline Button:** transparent, 1px `#23252a` border, text `#d0d6e0`, radius 6px.
- **Sign-up Button (White Pill):** bg `#ffffff`, text `#08090a`, radius 9999px, 13px/510.
- **Card (Product Screenshot Frame):** bg `#0f1011`, radius 12px, inset border `rgb(35,37,42)` 1px, padding 24px, no outer shadow.
- **Card (Subtle):** `rgba(255,255,255,0.02)` bg, radius 6px, shadow `rgba(0,0,0,0.4) 0 2px 4px`.
- **Text Input:** `rgba(255,255,255,0.02)` bg, 1px `rgba(255,255,255,0.08)` border, radius 6px, focus ring brightens border to `#d0d6e0`.
- **Badge / Status Tag:** `rgba(255,255,255,0.05)` bg, text `#8a8f98`, radius 4px, 12px/400; color variants use Pulse Green / Coral Red / Iris Violet / Lavender.
- **Logo Bar (Customer Strip):** neutral grey logos (Vercel, Cursor, Oscar, OpenAI, Coinbase…) at `#8a8f98`–`#d0d6e0`, 48–64px gaps, no cards.
- **Hero Gradient Floor:** linear gradient `rgb(8,9,10)` 10% → `rgb(208,214,224)` 100%, atmospheric base under the hero screenshot.

## Do's and Don'ts

**Do**
- Use Inter Variable with `cv01/ss03/zero` on — defines Linear's typographic identity.
- Use `#e4f222` for exactly one primary action per view, never decoration.
- Body text 16px/400/1.5; larger 17px+/590 only for emphasis blocks.
- Tight tracking (-0.022em) at 48px+ is non-negotiable for display type.
- Three-radius system only: 12px cards, 6px buttons, 9999px pills.
- Hairline borders (0.5px `#23252a`/`#383b3f`) instead of shadows for separation.
- Section gaps 96px, element gaps 8px — the 8/12/24/96 rhythm.

**Don't**
- No bold (700+) weights — caps at 590.
- No decorative gradients on buttons/cards/text — gradient reserved for the hero floor.
- No second chromatic accent as an action color.
- No radii above 12px on cards/panels.
- No shadows to separate cards — hairline borders + inset shadow only.
- No chromatic body text — stays in the grey scale.
- Berkeley Mono only for IDs/shortcuts/metadata, never headings.

## Surfaces & Elevation

| Level | Name | Value |
|---|---|---|
| 0 | Void | `#08090a` |
| 1 | Carbon | `#0f1011` |
| 2 | Obsidian | `#161718` |
| 3 | Slate | `#23252a` |

Elevation comes from hairline borders and subtle dark shadows (`rgba(0,0,0,0.4) 0 2px 4px`), not layered shadow stacks. The acid-lime CTA is the only chrome element with a real inset shadow stack.

## Imagery & Layout

Product-screenshot-first: real Linear UI (issue cards, kanban boards, AI agent panels) inside hairline-bordered frames — no stock photography, no illustration. Max-width ~1200px, full-bleed dark background. Hero: left-aligned 64–72px headline + right-aligned link CTA + large product screenshot bleeding past max-width. 96px section rhythm, low information density, single focal point per screen. Fixed top nav, no sidebar, no mega-menu.

## Similar Brands
Vercel, Cursor, Raycast, Framer — shared dark-canvas, hairline-border, single-accent-color language.

---

# Slack — Style Reference
> Aubergine stage with white spotlights. Deep plum dominates dark sections while a near-white canvas lets oversized Avant-Garde headlines breathe.

**Theme:** light

Slack's design language balances a near-white canvas with concentrated pools of aubergine purple — the brand color appears sparingly as CTA fills, dark hero sections, and gradient text highlights while the majority of the page stays airy and monochrome. Type is split into two voices: a geometric display face (Avant-Garde) for oversized headlines at 64-96px, and a humanist sans (Sans) for everything else. Sections alternate between flat white, faintly lilac washes (`#f9f0ff`), and fully inverted purple bands, with 16px-radius cards floating over a very subtle 32px ambient shadow.

## Tokens — Colors

| Name | Value | Role |
|------|-------|------|
| Aubergine | `#611f69` | Filled CTA buttons, primary nav fills, dark hero backgrounds |
| Deep Plum | `#481a54` | Full-bleed dark section backgrounds |
| Purple Haze | `#f9f0ff` | Softest lilac wash for body backgrounds, pill fills, card surfaces |
| Lavender Mist | `#eac8fe` | Card borders, decorative outlines, pill borders |
| Vivid Violet | `linear-gradient(104deg,#000 9.56%,#ba01ff 102.66%)` | Headline gradient-text accent on dark sections |
| Plum Shadow | `#3d0157` | Button text/shadow tones on aubergine surfaces |
| Channel Blue | `#1264a3` | Slack's in-product channel-link blue (product UI only) |
| Carbon | `#1d1c1d` | Primary body/nav text |
| Charcoal | `#454245` | Secondary body text |
| Mid Gray | `#696969` | Nav text, subdued labels |
| Fog | `#edeaed` | Hairline borders, dividers |
| Soft White | `#fefbff` | Page canvas |

## Typography

**Salesforce-Avant-Garde** (display/headings, geometric wide, 18–96px, weights 400/600/700) · **Salesforce-Sans** (body/UI, 12–23px, weights 300/400/600/700). Body 16px/1.5. Eyebrow labels: 12px/700, 0.057em uppercase tracking.

| Role | Size | Line Height |
|---|---|---|
| eyebrow | 12px | 1.5 |
| body | 18px | 1.56 |
| subheading | 32px | 1.25 |
| heading | 64px | 1.12 |
| display | 96px | 1.08 |

## Spacing & Shape
Radius: cards 16px · pills 999px · buttons 4px (rectangular, never pill for primary CTA). Max-width 1200px, section gap 80–100px.

## Components

- **Primary CTA (Aubergine Fill):** `#611f69` bg, white text 16px/700, **4px radius** (rectangular, not pill).
- **Ghost CTA:** transparent, `#3d0157` text, same padding.
- **Feature Card (Lavender Border):** transparent bg, 1px `#eac8fe` border, 16px radius, no shadow.
- **Product Screenshot Card:** 16px radius, floating with `rgba(0,0,0,0.1) 0 0 32px` shadow.
- **Dark Hero Band:** `#481a54` bg, white 64px/700 headline, scattered white four-point star decorations, soft radial color washes at 25% opacity.
- **Gradient Text Highlight:** single keywords use the black→violet gradient text-fill, never full headlines or body.

## Do's and Don'ts
**Do** reserve `#611f69` for filled CTAs only (use `#481a54` for large surfaces); set headlines 64–96px with -0.012em tracking; 16px radius + lavender border for default cards; 32px ambient shadow only on product/floating cards.
**Don't** use pill-radius on primary CTAs (always 4px rectangular); use Channel Blue in marketing CTAs; add shadows to hero band text; use gradients on UI surfaces (text-only).

## Layout
Max-width 1200px. Hero: centered 64px headline + twin CTAs (filled+ghost) + trust-logo strip + floating product screenshot. Bands alternate white → `#481a54` dark → white → `#f9f0ff` wash. 96px section gaps.

## Similar Brands
Linear, Notion, Webflow, Stripe.

---

# Calendly.com — Style Reference
> Navy ink on cool marble.

**Theme:** light

Calendly reads as a quiet, confident scheduling workspace: a near-white canvas with generous breathing room, crisp white product cards floating on cool stone-gray, and all typography rendered in deep navy ink (`#0b3558`) rather than pure black. A single vivid blue (`#006bff`) carries every primary action, while decorative pink and cyan blobs bleed from behind product mockups to add warmth.

## Tokens — Colors

| Name | Value | Role |
|------|-------|------|
| Ink Navy | `#0b3558` | Primary text, headings, icons, dark CTA backgrounds |
| Signal Blue | `#006bff` | Primary CTA fill, active nav, links |
| Slate Gray | `#476788` | Secondary body copy |
| Mist Gray | `#a6bbd1` | Disabled text, inactive labels |
| Cloud | `#f8f9fb` | Page canvas |
| Paper | `#ffffff` | Card surfaces |
| Hairline | `#d4e0ed` | Borders, dividers |
| Coral Magenta | `#e55cff` | Decorative accent blob behind product cards |
| Sky Cyan | `#0099ff` | Decorative accent blob (paired with magenta) |

## Typography
**Gilroy** — sole family. Weights 400/500/600/700. Display headlines 68–80px (unusually large for SaaS, gives editorial weight). Body 16px.

| Role | Size |
|---|---|
| body | 16px |
| button | 18px |
| heading | 50px |
| heading-lg | 68px |
| display | 80px |

## Spacing & Shape
Base 8px. Radius: cards 24px · product cards 16px · buttons/inputs 8px · badges 9999px.

## Components
- **Primary CTA:** `#006bff` bg, white text 18px/600, 8px radius.
- **Dark CTA:** `#0b3558` bg, white text — secondary filled action.
- **Elevated Product Card:** white, 16px radius, three-layer blue-tinted shadow `rgba(71,103,136,...)`, often fronted by a magenta/cyan blob.
- **Social Sign-In Button:** full-width pill-ish, Google (white/navy/1px border) or Microsoft (navy/white, no border).
- **Booking Widget Card:** white, 16px radius, mimics the real product (organizer info + date grid + time-slot pills in `#006bff`).

## Do's and Don'ts
**Do** use Ink Navy for all text (never pure black); Signal Blue only for filled primary CTAs; blue-tinted shadow stack on every elevated surface; 16px product-card / 24px feature-card radii.
**Don't** use `#000000` anywhere; use neutral-black shadows; use decorative blobs as functional UI fills; go below 38px on H2 headings.

## Layout
Max-width 1200px. Hero: two-column (headline+CTA left, booking widget card right on blobs). Trust logo strip below. Feature sections pair text with product visuals; 48–64px section gaps.

## Similar Brands
Linear, Notion, Loom, Webflow.

---

# Atlassian — Style Reference
> Confetti-edged engineering blueprint. A clean white enterprise canvas interrupted by dark navy editorial panels framed in torn geometric color.

**Theme:** light

Atlassian pairs a white enterprise canvas with expressive dark hero blocks framed by fragmented geometric "confetti" in vivid violet, taxicab yellow, electric blue, and green. One electric blue (`#1868db`) drives every primary action and link; chromatic energy lives only in decorative edges, never functional UI.

## Tokens — Colors

| Name | Value | Role |
|------|-------|------|
| Atlassian Blue | `#1868db` | Single chromatic action color — buttons, links, focus states |
| Midnight Navy | `#101214` | Primary text, dark hero panel backgrounds |
| Taxicab Yellow | `#fca700` | Decorative confetti, CTA on dark hero only |
| Lavender Wash | `#eed7fc` | Editorial section-divider backgrounds |
| Confetti Gradient | conic violet→yellow→blue | Decorative frame around video/hero blocks |
| Fog White | `#f0f1f2` | Muted button backgrounds, hairline dividers |

## Typography
**Charlie Display** (editorial headlines, 14–80px, weights 400/500/700/800) · **Charlie Text** (body/UI, 13–24px, weights 400/500/700). Display 80px at 0.012em tracking.

## Spacing & Shape
Radius: nav 2px · tags 10000px (pill) · cards 20px · buttons 28px (near-pill). Max-width 1200px, section gap 64–80px.

## Components
- **Primary Action Button:** `#1868db` fill, white text, 28px pill radius, zero shadow.
- **Dark Hero Banner:** `#101214` bg framed by jagged violet/yellow/blue/green confetti shapes; yellow CTA is the only place yellow appears as a button.
- **Product Screenshot Card:** screenshot tilted slightly on solid `#1868db` background — the blue IS the frame.
- **Lavender Feature Band:** `#eed7fc` full-width, text floats directly on the tint, no card containers.
- **Card Container:** white, 20px radius, minimal 1px `#f0f1f2` border or navy-tinted micro-shadow, no drop shadow at scale.

## Do's and Don'ts
**Do** keep `#1868db` as the only action color; 20px card / 28px button radii; confetti (violet/yellow/blue/green) only around dark panels, never inside functional UI; navy-tinted shadow stack `rgba(9,30,66,...)` for any elevation.
**Don't** use yellow/violet/green on buttons/links/forms; use heavy shadows (system is flat); use sharp corners on cards/images; use pure `#000000` as a fill.

## Layout
Alternating white/lavender bands with occasional full-bleed dark navy panels. Content max-width 1200px. Hero: full-bleed dark panel, confetti bleeding off-page edges. Sticky top nav with mega-menus. 64–80px between major sections.

## Similar Brands
Notion, Linear, Figma, GitHub, Slack.

---

# Generative AI (fal) — Style Reference
> 8-bit playground on clean white paper. A white canvas interrupted by flat colored bands and scattered pixel-art creatures, held together by one bold geometric typeface and zero shadows.

**Theme:** light

fal uses a playful generative-canvas language for a developer-tool audience: clean white surfaces, one bold geometric sans (**focal**) at compressed tracking, dark filled buttons against brightly-colored full-bleed section bands (sky-blue hero, lime highlight, violet CTA strip, pink testimonial accent), and scattered 8-bit pixel-art creatures in lime/violet/pink. Components stay flat and sharp — 4px button radii, 12px card radii, hairline `#e5e7eb` borders, **no shadows, no gradients, no pill controls**.

## Tokens — Colors

| Name | Value | Role |
|---|---|---|
| Sky Cyan | `#99ecff` | Hero band background, full-bleed section wash |
| Electric Violet | `#6120ee` | Inline links, brand chromatic |
| Deep Ultraviolet | `#4a17b0` | Dark CTA strip background |
| Pixel Lime | `#f1ffd2` | Decorative highlight band / pixel-art fill |
| Bubblegum Pink | `#ffddfa` | Testimonial-section accent |
| Carbon | `#252527` | Dark filled button — the only button fill color |
| Graphite | `#1b1b1d` | Primary text, nav links |
| Hairline Gray | `#e5e7eb` | Universal border/divider — the only structural border color |

## Typography
**focal** (display/heading/body, 10–120px, weights 400–700, tight negative tracking that scales with size) · **Chivo Mono** (code) · **publicSansRounded** (buttons/tags/nav CTAs, rounded terminals, 14–24px).

## Spacing & Shape
Base 8px grid: 8/16/24/32/48/64/96/112/128px. Radius: buttons/inputs/tags 4px · cards 8–12px · images 4–8px. **No pill shapes anywhere.**

## Components
- **Dark Filled Button:** `#252527` bg, white text, 4px radius, no shadow, no hover-lift — must feel like a printed label.
- **White Outlined Button:** white bg, 1px `#1b1b1d` border, inverts on hover.
- **Hero Section:** `#99ecff` full-bleed, 80px `focal` weight-700 headline at ~50% width, pixel-art creatures bleeding off edges.
- **Model Gallery Card:** 3:4 image fills card edge-to-edge, 12px radius, bottom-gradient text overlay, no border.
- **Pixel Art Decoration:** 8–16px square blocks in lime/lavender/pink/yellow with dark outlines — the only imagery besides model cards; positioned absolutely, overlapping content.

## Do's and Don'ts
**Do** use focal at 60–80px/700 for headlines; `#99ecff` only as full-bleed band, never a swatch; 8px spacing grid discipline; 12px card / 4px button radii; pixel-art decorations in hero/dark bands.
**Don't** use chromatic CTA fills (always neutral `#252527`); add shadows or gradients anywhere; use rounded/pill shapes; break the 8px grid; use pixel-art colors as functional UI colors.

## Layout
Max-width 1200px on full-bleed white canvas. Hero is a full-viewport cyan band; sections alternate white/colored full-bleed bands. Two-column text blocks, 4-column model-card grids. 64–80px section rhythm.

## Similar Brands
Together AI, Replicate, Runway, Vercel, Perplexity.

---

# Leonardo.ai — Style Reference
> Inverted editorial gallery. A black-walled museum where 165px violet headlines act as wall installations and AI-generated portraits hang in a tight grid below.

**Theme:** dark

Leonardo.ai is a cinematic dark-mode creative arena: near-black canvas (`#000000`) is an infinite gallery floor; the interface speaks through sheer typographic mass rather than chrome. One saturated violet (`#6e60ee`) is the brand identity color, surrounded by a vivid six-color tag palette (green/violet/yellow/pink/coral/blue) used strictly as categorical color-coding. Display type reaches **165px** with compressed line-heights (0.80–0.90) and tight tracking — headlines are sculptural objects.

## Tokens — Colors

| Name | Value | Role |
|---|---|---|
| Midnight Canvas | `#000000` | Page background |
| Charcoal Card | `#353535` | Card/gallery-image surface |
| Leonardo Violet | `#6e60ee` | Brand identity — logo, active tab, brand highlights (identity, not decoration) |
| Toxic Lime / Voltage Yellow / Shock Pink / Ember Coral / Plasma Pink / Arc Blue | six accents | Tag-chip taxonomy only — never large fills |
| Bone White | `#ffffff` | Primary text, filled primary-action background |

## Typography
**leoSans** (display, 34–165px, weights 500/800/900, line-height 0.80–0.93, tracking to -0.02em) · **canvaSans** (UI/body, 10–19px, weights 400/500/700).

## Spacing & Shape
Radius: buttons 60px (full pill) · cards 8px · tags 270px. Max-width 1440px, section gap 80px.

## Components
- **Primary CTA (Filled Pill):** white bg, black text, 60px radius — the only filled button, white-on-black IS the elevation.
- **Active Tab Pill:** `#6e60ee` fill, glow `0 0 24px rgba(110,96,238,0.45)`.
- **Gallery Image Card:** `#353535` bg, 8px radius, image bleeds to edge, no padding — 3–4 column grid, 10–14px gaps.
- **Category Tag Chip:** pill, one of the six accent colors, white text 12–14px/700 — color IS the taxonomy.
- **Hero Display Wordmark:** leoSans 900 at 90–165px, `#6e60ee`, sometimes perspective-warped — a graphic object, not a heading.

## Do's and Don'ts
**Do** use 60px pill radius for all buttons/active tabs; push display type to 90px+ at 0.80–0.90 line-height; keep `#6e60ee` for identity only; six-accent palette for tag chips exclusively; `#000000`→`#353535` as the entire surface ramp.
**Don't** put the white pill on non-black surfaces; use the accent palette for large fills/backgrounds; exceed 1.0 line-height on leoSans; mix card radius (8px) with button radius (60px); add shadows beyond 1px on dark surfaces.

## Layout
Max-width 1440px on full-bleed black. Hero is a full-viewport sculptural typography piece; sections alternate 3–4 column image grids and centered text with tag pills. Minimal transparent nav. 80px section gaps, 10px element gaps.

## Similar Brands
Midjourney, Runway, NightCafe Creator, Pika, Stability AI.

---

# Morphic — Style Reference
> Dark cinema canvas for AI storytelling. Pure black absorbs everything except the blue pulse of a single accent and the glow of generated imagery.

**Theme:** dark

Morphic is 99% achromatic: a tightly stepped neutral stack `#000000` → `#212121` → `#292929` → `#333333` carries the interface. A single vivid blue (`#0075ff`) is the only chromatic accent — reserved for primary actions and the "New" badge, functioning as an electrical pulse. Every major section header uses a signature **two-tone headline**: line 1 white, line 2 muted gray as a descriptive echo.

## Tokens — Colors

| Name | Value | Role |
|---|---|---|
| Pure Black | `#000000` | Page canvas |
| Surface One/Two/Three | `#212121`/`#292929`/`#333333` | Card → raised → floating elevation steps |
| Paper White | `#ffffff` | Headings, buttons, high-emphasis text |
| Mid Gray | `#999999` | Muted body text — **all body copy uses this, never white** |
| Electric Blue | `#0075ff` | The single chromatic accent — CTAs and "New" badge only |

## Typography
**Inter** only, all weights 400–700. Display 52px at -0.062em tracking; headings 40px at -0.048em.

## Spacing & Shape
Radius: buttons/badges 7px · cards 10px · large cards 16px · modals 24px · pills 100px. Max-width 1280px, section gap 96px.

## Components
- **Primary CTA Button:** `#0075ff` fill, white text 14px/500, 7px radius — the only filled chromatic element.
- **Secondary Button:** `#292929` fill (one surface step up), same text spec.
- **Two-Tone Headline:** line 1 white / line 2 `#999999`, same size/weight — repeats across every section, the brand's signature device.
- **Image Showcase Card:** no border, 10px radius, image fills edge-to-edge, optional soft shadow only here.
- **New Badge:** `#0075ff` fill, white text, 7px radius, inline with copy.

## Do's and Don'ts
**Do** use `#0075ff` exclusively for primary actions/badge; apply the two-tone headline pattern everywhere; stick to the exact 4-step surface ramp; -0.062em tracking at 52px.
**Don't** introduce a second chromatic color; add shadows to UI components (only image cards); use white for body copy (always `#999999`); center body paragraphs; use gradients anywhere.

## Layout
Full-bleed black, max-width ~1280px. Hero: two-column (two-tone headline + dual CTAs left, nothing right but void). Showcase grid: 2-row × 7-column borderless image cards. Horizontal-scrolling workflow carousels below. 96px section gaps.

## Similar Brands
Runway ML, Midjourney, Pika, ElevenLabs, Stability AI.

---

# Apple — Style Reference
> white room with a single blue switch.

**Theme:** light

Apple's design language is a study in restraint: near-white canvas, generous breathing room, and one vivid blue accent (`#0071e3`) that makes every action feel deliberate. Typography is the primary voice — SF Pro set with negative tracking that tightens as size grows. The product IS the design: large product photography dominates, while chrome recedes into thin borders and hairline rules.

## Tokens — Colors

| Name | Value | Role |
|---|---|---|
| Apple Blue | `#0071e3` | Filled action buttons — the only chromatic interactive color |
| Link Blue | `#0066cc` | Outlined action borders, inline links |
| Signal Blue | `#2997ff` | Decorative borders/strokes only |
| Carbon | `#1d1d1f` | Primary text |
| Frost | `#f5f5f7` | Page canvas — the signature Apple light gray |
| Pebble | `#e2e2e5` | Button fills, disabled surfaces |

## Typography
**SF Pro Display** (headlines 21–56px, weights 400/600/700) · **SF Pro Text** (body/nav/buttons, 12–44px, weights 300/400/600). Body 17px at -0.016em tracking.

## Spacing & Shape
Radius: cards/images/inputs 8px · buttons/tags **980px (full pill)** — the only two radii in the whole system. Max-width 1440px, section gap 64px.

## Components
- **Filled Pill Button:** `#0071e3` bg, white text 17px/400, 980px radius, no shadow — the single filled interactive element.
- **Outlined Pill Button:** 1px `#0066cc` border, transparent fill — always paired next to the filled button.
- **Product Hero Section:** `#f5f5f7` bg, 56px/600 centered name, 26px/300 tagline, two pill buttons, large product render.
- **Feature Banner:** full-bleed photographic/color-wash background — the image IS the surface, no card container.

## Do's and Don'ts
**Do** use `#0071e3` only for filled buttons/selected states; pair every filled button with an outlined secondary; 980px radius for every interactive element; full-bleed `#f5f5f7` sections with no cards inside.
**Don't** use `#0071e3` for text/borders/decoration; add drop shadows to cards/buttons/nav; use 700-weight headlines for product names (max 600); use radius below 980px on buttons or above 8px on cards/images.

## Layout
Full-bleed, no fixed max-width container; text blocks center internally at ~980px. Hero always centered: name → tagline → two pills → product render. 64px+ vertical rhythm between `#f5f5f7`/color-wash bands. No sidebars, everything centered and symmetrical.

## Similar Brands
Bang & Olufsen, Teenage Engineering, Nothing, Dyson.

---

# Superhuman — Style Reference
> golden hour editorial dashboard

**Theme:** light

Superhuman sits between editorial photography and software UI — a warm parchment canvas (`#f2f0eb`, never pure white) frames deep-maroon brand moments and vivid violet accents. Headlines whisper at **weight 460** rather than shout, letting a cinematic full-bleed hero photograph carry the emotion while translucent product-UI cards float like glass over the image. No heavy shadows or gradients on UI surfaces — depth comes from layered photography.

## Tokens — Colors

| Name | Value | Role |
|---|---|---|
| Midnight Wine | `#421d24` | Primary action buttons, announcement banner, footer |
| Royal Violet | `#714cb6` | Inline links only — never a button fill |
| Lilac Mist | `#d4c7ff` | Secondary surface fills, ghost button backgrounds |
| Warm Parchment | `#f2f0eb` | Page canvas — replaces white as the base |
| Ink Charcoal | `#292827` | Primary text — warm near-black, never pure `#000` |
| Deep Lagoon | `#0c4243` | The one dark full-bleed feature-band background |

## Typography
**Super Sans VF** — sole typeface, variable weight 460 (signature light-cut voice for display) through 540/600/700. Display 64px at -0.028em.

## Spacing & Shape
Radius: buttons/cards/floating-cards 16px · tabs/small-buttons 8px · pills 999px. Max-width 1200px, section gap 64–96px.

## Components
- **Primary Action Button:** `#421d24` fill, white text 16px/460, 16px radius — the only chromatic button fill.
- **Floating Product Card:** white at ~85% opacity, 16px radius, no drop shadow — composited directly over hero photography (the system's signature move).
- **Outlined Light Button:** `#d4c7ff` fill, `#292827` text + border, 8px radius — secondary tier.
- **Dark Feature Band:** `#0c4243` full-bleed, layered translucent geometric shapes + handwritten-script overlay on one side.

## Do's and Don'ts
**Do** use weight 460 for all headlines 28px+; body text `#292827` on `#f2f0eb` canvas (never pure white full-page bg); `#421d24` as the single primary fill; violet exclusively for inline links; float cards over photos with no shadow.
**Don't** use weight 700+ for headlines; place white-on-white; add drop shadows to cards; introduce a blue/green/red accent; center body copy over two lines; use pure `#000000` text.

## Layout
Full-bleed cinematic photo hero with floating translucent product cards; white logo strip; suite-tabs section; one dark teal band two-thirds down; gradient atmospheric band; maroon footer. 64–96px section rhythm, max-width ~1200px.

## Similar Brands
Notion, Arc Browser, Linear, Stripe, Causal.

---

# WhatsApp.com — Style Reference
> sunlit coffee shop conversation

**Theme:** light

WhatsApp's marketing site reads as a warm, human messaging app: a soft cream backdrop (`#fcf5eb`) carries the whole page, letting full-bleed photography and oversized typography (up to 80px) do the talking while a single vivid green (`#25d366`) punctuates every action. Components are generous and soft: **50px pill buttons, 25px rounded image cards, no shadows anywhere.**

## Tokens — Colors

| Name | Value | Role |
|---|---|---|
| WhatsApp Green | `#25d366` | Primary CTA — the singular chromatic accent, action-only |
| Link Blue | `#0373e9` | Inline text links exclusively — never a fill |
| Charcoal | `#1c1e21` | High-contrast text/border color |
| Cream Canvas | `#fcf5eb` | Page background — warm off-white, not pure white |
| Pure White | `#ffffff` | Card surfaces, chat bubbles |

## Typography
**WhatsApp Sans Var** — sole typeface, only two weights (400 body/UI, 700 display). Display reaches 80px at line-height 1.0 — a deliberately dramatic 5× jump from 16px body.

## Spacing & Shape
Radius: buttons/inputs **50px (full pill)** · images **25px** · cards 16px. Max-width 1200px, section gap 120–160px.

## Components
- **Primary CTA (Pill):** `#25d366` fill, white text 16px/700, 50px radius, download-arrow icon.
- **Ghost Nav Button:** transparent, 1px `#1c1e21` border, 50px radius.
- **Chat Bubble (Incoming/Outgoing):** white or light-green (`#d9fdd3`) fill, 8px radius, floats freely as atmospheric UI decoration.
- **Feature Image Card:** 25px radius, no border/shadow, photo fills edge-to-edge.

## Do's and Don'ts
**Do** use `#25d366` for exactly one CTA per viewport; 50px radius on all buttons/tags; let cream canvas show through generously; 25px radius on all imagery; keep `#0373e9` for inline links only.
**Don't** use green for icons/decoration; introduce new chromatic colors; use sharp corners (0–4px) anywhere; add drop shadows; set headlines below 48px; use pure `#000000` text.

## Layout
Full-bleed photographic hero with headline anchored left + chat bubbles floating right. Generous cream whitespace between feature sections (120–160px gaps). Clean top bar: logo, links, ghost Log In + green Download CTA.

## Similar Brands
Apple product pages, Headspace, Duolingo, Notion.

---

# Mobbin — Style Reference
> Grayscale specimen board — a printer's proof sheet where typographic weight IS color.

**Theme:** light

Mobbin runs on pure achromatic restraint — **zero chroma** across the entire palette, forcing hierarchy through weight, size, and tone alone. Near-black ink (`#141414`) at display sizes, warm-gray secondary text. The custom **saans** typeface uses fractional weights (440, 456, 652) that don't exist in system fonts — typography doing the work color usually does. 9999px pill shapes on every interactive element; app-screenshot cards ARE the visual texture of the page.

## Tokens — Colors

| Name | Value | Role |
|---|---|---|
| Midnight Ink | `#141414` | The single "color" — all buttons, active states, headings |
| Pure Canvas | `#ffffff` | Page background |
| Graphite | `#707070` | Body copy |
| Ash | `#adadad` | Tertiary/disabled text |
| Fog | `#ededed` | Card borders (elevation via border, never shadow) |

## Typography
**saans** — fractional weights 400/440/456/600/652 mapped to semantic roles (440 = UI labels, 456 = mid-emphasis body, 652 = hero numerics). Display 80px at -0.88px tracking, centered always.

## Spacing & Shape
Base 8px. Radius: buttons/inputs/tags **9999px** · cards/thumbnails 16px · modals 24px. Max-width 1280px, section gap 80px.

## Components
- **Primary Filled Button:** `#141414` bg, white text, 9999px radius.
- **App Screenshot Card:** white, 1px `#ededed` border, 16px radius — phone screenshot fills upper portion, "New" pill badge overlay.
- **Filter Pill Row:** active = `#141414` fill/white text; inactive = transparent + `#141414` border — pill shape throughout.
- **Section Stat Display:** 56–80px saans/652 numeric centerpiece, no decoration.

## Do's and Don'ts
**Do** treat `#141414` as the only color in the system; 9999px on every interactive pill, 16–24px on containers; fractional weights 440/456/652 (never round to 400/500/600); borders (not shadows) for card elevation.
**Don't** introduce any chromatic accent (no blue links, no green success states); use box-shadow on cards; use weight 700/800; use radius values outside the fixed set; left-align hero headlines (always centered).

## Layout
Max-width ~1280px, white throughout. Centered hero: display headline → subtitle → two pill CTAs → app-icon specimen. Trust logo bar. Sticky secondary nav (tabs + search + filters) above a 3-column screenshot grid. 80px section rhythm, no alternating dark/light bands.

## Similar Brands
Screenlane, Dribbble, Lookup.design, Linear, Refero.design.

---

## 如何更新本文档

本文档由 [Refero Styles](https://styles.refero.design/) 人工挑选整理而成（该站点收录 2000+ 套设计系统，覆盖 SaaS、AI、消费级 App、企业软件等品类）。如需补充新的风格参考：

1. 打开 https://styles.refero.design/ ，用站内搜索框按品牌名或关键词（如 `SaaS`、`AI`、`premium`）查找目标网站的设计系统页面。
2. 打开对应的 `/style/{id}` 详情页，切换到 **DESIGN.md** 标签页，点击 **Copy** 复制完整内容。
3. 按本文件的分区格式粘贴进来，并在目录中补充一条索引。

> 注：该站点的 `robots.txt` 对已知 AI 爬虫整体禁止抓取，仅允许通过浏览器交互式访问（即按钮点击 + 复制），因此本文档以人工浏览 + 复制的方式整理，未做自动化批量抓取。
