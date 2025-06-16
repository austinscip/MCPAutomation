Build the **MCP Server Auto-Deployment module** for the “MCP Automation Studio.” When a user’s workflow includes a platform (e.g., Canva, Slack), this module should automatically locate, configure, and deploy the appropriate **open-source MCP server** (e.g., Anthropic’s Postgres-based Slack server).

Your output must include:

* Logic to **select the correct MCP server** based on the requested tool and available GitHub templates.  
* Automatic deployment pipeline (e.g., GitHub Actions or Docker) to install the server.  
* **Webhook** and **Zapier MCP SDK trigger integration**, with real-world MCP formats.  
* Embedded **Claude-generated server metadata** (e.g., OpenAPI-compatible info, server ID, tags, usage constraints).

**Requirements:**

* Structure all code into **modular, reusable functions** designed for:  
  * **Bubble** (JavaScript plugin or API connector)  
  * **Zapier’s MCP SDK** (triggers/actions/searches)  
  * **Node.js/serverless/Express backends**  
* Avoid hardcoded values — use **parameters**, environment configs, or JSON-driven inputs.  
* For each function, include:  
  * Purpose (commented clearly)  
  * Sample inputs  
  * Sample outputs (with JSON schemas or API response shape)  
  * Brief real-world usage example (e.g., “auto-deploy Claude-to-Slack MCP server from GitHub”)

**Focus areas:**

* Production-ready backend logic  
* GitHub-based deployment using Docker or prebuilt workflows  
* Real MCP server metadata generation  
* Plug-and-play extensibility (supporting 5,000+ MCP servers)