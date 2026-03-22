# Design System Document: The Editorial Precision Framework

## 1. Overview & Creative North Star
### Creative North Star: "The Informed Curator"
In an era of digital noise, Janta Media & Communications Services must stand as a beacon of clarity and authority. This design system departs from the standard "blocky" corporate template in favor of an **Editorial Precision** aesthetic. Think of it as a premium high-end magazine met with modern digital fluidity.

We achieve this through:
*   **Intentional Asymmetry:** Breaking the grid to draw the eye to key narratives.
*   **Tonal Depth:** Moving away from flat colors to layered, tactile surfaces.
*   **Micro-Typography:** Using scale and whitespace as functional structural elements rather than just decoration.

The goal is a "significant upgrade" that feels intentional, where every pixel serves the story of professional media services.

---

## 2. Colors: Tonal Depth & Soul
Our palette transitions from simple Navy and Gold to a sophisticated spectrum of depths.

### The Palette
*   **Primary (Deep Authority):** `#000823` (Primary) to `#011D52` (Primary Container). Use these for deep-immersion sections.
*   **Secondary (The Golden Thread):** `#785900` (Secondary) and `#ffc73c` (Secondary Container). Gold is used as a "surgical" highlight, never a background wash.
*   **Surface Hierarchy:** We use `surface-container-lowest` (#ffffff) through `highest` (#dfe2f0) to define sections.

### The "No-Line" Rule
**Explicit Instruction:** Prohibit 1px solid borders for sectioning. Boundaries must be defined solely through background color shifts. For example, a `surface-container-low` section sitting against a `surface` background provides a sophisticated, modern transition that looks "designed," not "constructed."

### The Glass & Gradient Rule
To ensure the site feels premium:
*   **Glassmorphism:** Use for floating navigation or overlay cards. Use `surface-container-lowest` at 70% opacity with a `20px` backdrop-blur.
*   **Signature Textures:** Apply a subtle linear gradient (Top-Left to Bottom-Right) from `primary` (#000823) to `primary-container` (#011d52) for Hero backgrounds. This prevents the "flat-bucket-fill" look and adds a sense of atmospheric depth.

---

## 3. Typography: The Editorial Voice
We utilize a high-contrast scale to create an immediate hierarchy of information.

*   **Display (Manrope):** Large-scale, tight tracking. Use `display-lg` (3.5rem) for hero statements to evoke the feeling of a magazine masthead.
*   **Headline (Manrope):** Clean and authoritative. Headlines should always use the `on-background` (#171b25) color to maintain high legibility.
*   **Body (Inter):** Chosen for its exceptional readability at smaller scales. Use `body-lg` (1rem) for general copy and `body-sm` (0.75rem) for meta-data or captions.
*   **Label (Inter):** All-caps with increased letter spacing (0.05em) for category tags or small "eyebrow" text above headlines.

---

## 4. Elevation & Depth: Tonal Layering
Traditional shadows and borders are replaced with **Tonal Layering**.

*   **The Layering Principle:** Depth is achieved by "stacking" surface tiers. Place a `surface-container-lowest` card on a `surface-container-low` section. This creates a soft, natural lift without the "dirty" look of heavy shadows.
*   **Ambient Shadows:** For floating elements (like the "Accept" cookie banner), use a shadow with a large blur (32px) at 6% opacity, tinted with the `on-surface` color. It should feel like a soft glow, not a hard drop.
*   **The Ghost Border Fallback:** If a container needs more definition (e.g., on a white background), use a "Ghost Border": the `outline-variant` token at 15% opacity. Never use 100% opaque borders.
*   **Glassmorphism:** Use backdrop blurs on the main navigation bar to allow the hero imagery to bleed through, softening the transition from header to content.

---

## 5. Components: Refined Interactions

### Buttons (The Interaction Points)
*   **Primary:** Solid `secondary-container` (#ffc73c) with `on-secondary-container` (#705300) text. Use `xl` (0.75rem) roundedness. 
*   **Tertiary:** No background. Use `primary` text with a 2px underline in `secondary` that appears on hover.

### Cards & Lists
*   **Rule:** Forbid divider lines. Use vertical whitespace (Spacing Scale `12` or `16`) or subtle background shifts (`surface-container-lowest` cards on a `surface-container-low` ground) to separate items.
*   **Media Cards:** Use a slight 1.02x scale-up on hover to indicate interactivity, paired with a transition-duration of 300ms.

### Input Fields
*   **Styling:** Use `surface-container-high` for the field background. No border. On focus, transition the background to `surface-container-highest` and add a `secondary` 2px bottom-bar.

### Floating Notices (Cookie/Privacy)
*   Instead of a full-width bar, use a floating "Toast" style card in the bottom-left. Style with `primary-container` background and `secondary-container` CTAs to maintain the brand’s high-contrast professional feel.

---

## 6. Do's and Don'ts

### Do:
*   **Do** use asymmetrical layouts where text blocks and images overlap slightly to create depth.
*   **Do** prioritize whitespace. If you think there's enough room between sections, double it.
*   **Do** use the "Golden Yellow" (`secondary`) sparingly—as a highlighter for key phrases or CTA buttons only.

### Don't:
*   **Don't** use 1px solid lines to separate content sections.
*   **Don't** use default black (#000000) for text; always use the `on-surface` or `primary` tokens for a softer, more premium contrast.
*   **Don't** center-align long blocks of text. Stick to left-aligned editorial layouts for a professional media feel.
*   **Don't** use sharp corners. Stick to the `xl` (0.75rem) or `full` roundedness scale to keep the interface feeling modern and approachable.