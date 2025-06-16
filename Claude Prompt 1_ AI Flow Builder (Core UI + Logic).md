Build the **AI Flow Builder module** for the “MCP Automation Studio.” The user types a natural language automation goal (e.g., “sync Shopify orders to QuickBooks invoices”), and the system parses it into a structured, editable, visual workflow.

Deliver:

* A frontend **input parser** that uses Claude to interpret the user's intent.  
* Backend logic that outputs a **JSON-based automation schema** (Bubble-compatible).  
* A **drag-and-drop visual builder** UI (suitable for Bubble or React embedding).  
* Editable **connectors**, **triggers**, and **steps** (e.g., Shopify → Claude → QuickBooks).

All components must be **modular and production-ready** — no placeholders or demo logic. Use real API references (e.g., Shopify, Slack, QuickBooks) wherever possible.

Structure:

* Code must be broken into **reusable functions** usable in:  
  * **Bubble plugins or API connectors**  
  * **Zapier MCP SDK** (as triggers/actions/searches)  
  * **Node.js / serverless backends**  
* Avoid hardcoding. Use parameters, fallback logic, and constants.  
* For each function, provide:  
  * A clear comment describing its purpose  
  * Sample inputs  
  * Expected outputs (with schemas or examples)  
  * Brief usage guide

Focus on:

* Maintainability  
* Extensibility (other platforms like Notion, X, or Epic)  
* Real-world deployability (Bubble, Zapier, serverless backend-ready)