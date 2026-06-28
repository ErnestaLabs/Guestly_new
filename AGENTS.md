
# CRITICAL RULES — NEVER BREAK THESE

## Hero Image Positioning (ABSOLUTE)
- The hero photo MUST start below the navigation bar. If the nav is `absolute top-0` with height `h-20`, the hero section/image must use `height: calc(100vh - 5rem); margin-top: 5rem` or equivalent to account for the nav overlap.
- Every hero image MUST have `object-top` in its class to prevent cropping the subject's head. Portrait photos of people will always have their face in the top portion.
- The nav and hero photo overlapping is the #1 most repeated mistake. Never let it happen again.

## Design Implementation
- Always implement against a DESIGN.md spec first. Never guess design tokens.
- No Lucide/FontAwesome icons unless customized.
- No colored icon backgrounds.
- No rounded corners (border-radius: 0) on form CTA buttons in dark sections.
- Transitions: 0.5s cubic-bezier(0.25, 1, 0.5, 1).
- CTAs: all caps, tracking-[0.18em], font-weight 500.
