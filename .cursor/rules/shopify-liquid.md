---
description: Applies when editing Shopify Liquid files to ensure OS 2.0 standards and performance.
globs: ["**/*.liquid", "sections/*.liquid", "snippets/*.liquid", "templates/*.json"]
---

# Shopify Liquid Standards 2026

- **Context Preservation:** Always check if a variable is available in the current scope before using it.
- [cite_start]**Performance:** - Never use `all_products` inside a loop[cite: 178].
    - [cite_start]Prefer `render` over `include`[cite: 108].
- [cite_start]**Schema:** Ensure all `{% schema %}` blocks are valid JSON and follow Shopify OS 2.0 standards[cite: 110].
- **Token Efficiency:** Keep explanations brief. [cite_start]Provide the code fix first, then a 1-sentence explanation[cite: 376, 420].