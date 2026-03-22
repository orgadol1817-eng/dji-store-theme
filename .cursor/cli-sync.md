---
description: EMERGENCY PROTOCOL: Triggered ONLY on Shopify CLI errors, EADDRINUSE, port conflicts, or sync freezing.
globs: ["*"]
---

# Shopify CLI Recovery Protocol

## 🔴 Trigger: `EADDRINUSE` / "Address already in use"
**Action:** The port (usually 9292) is deadlocked. 
Provide exactly this bash block and NOTHING else:
```bash
kill -9 $(lsof -ti :9292) && shopify theme dev