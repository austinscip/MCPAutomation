Build the **API Change Monitoring Module** for the MCP Automation Studio. This module ensures connected services stay functional when their APIs (especially OpenAPI-based) change. It must:

### **Core Features:**

* Automatically **track OpenAPI specs** of third-party services (e.g., QuickBooks, Shopify).  
* **Compare previous and updated specs** to detect:  
  * Removed/renamed endpoints  
  * Parameter/schema changes  
  * Auth or URL modifications  
* **Notify the user** via JSON output or UI hook if a change is detected.  
* **Suggest or auto-apply fixes** (e.g., route updates, param remapping) to workflows where changes break flows.

### **Code Requirements:**

* Structure all code into **modular, reusable functions** usable in:  
  * **Bubble** (via JavaScript plugin or API connector)  
  * **Zapier’s MCP SDK** (triggers/actions/searches)  
  * **Node.js/serverless/Express** apps  
* Avoid hardcoding — accept config/URLs as **parameters**  
* Each function must include:  
  * Clear purpose description  
  * Sample inputs and outputs (with JSON schemas)  
  * Real-world example (e.g., “Shopify spec changed `/inventory` param — module flags and suggests fix”)

### **Output format:**

* Functions return:  
  * JSON summary (e.g., `{ "changed": true, "diff": [...], "recommendedFix": {...} }`)  
  * Optionally, UI-triggerable actions (e.g., “Update Route”)

### **Implementation Notes:**

* Use real-world OpenAPI examples (e.g., Swagger JSON from Shopify/QuickBooks).  
* Support diffing via spec parser (e.g., `swagger-parser`, `diff-openapi`).  
* Designed for long-term monitoring (e.g., webhook to trigger when new spec is detected).