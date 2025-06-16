Build the **Blueprint Marketplace Module** for the AI-Powered MCP Automation Studio. This marketplace allows users to upload and sell automation blueprints, set pricing, and receive royalties. It must include user-friendly frontends and backend services compatible with low-code tools.

---

### **✅ Functional Requirements:**

1. **Blueprint Upload & Download System**  
   * Upload workflow blueprint files (e.g., JSON or YAML format)  
   * Store metadata: title, category, industry, use-case tags  
   * Download system with usage logging  
2. **Pricing & Royalty Logic**  
   * Users can set a price from **$5–$25**  
   * System deducts **15–25% marketplace fee**  
   * Remaining goes to seller via Stripe, PayPal, or token wallet  
3. **Claude-Generated Metadata**  
   * Auto-generate:  
     * Blueprint descriptions (clear, benefits-driven)  
     * Compliance tags (e.g., HIPAA, GDPR, SOC2) based on blueprint content  
   * Claude input: uploaded blueprint, user-provided tags  
   * Output: JSON with title, description, labels  
4. **Bubble-Compatible Flows & Frontend**  
   * Components to:  
     * Browse/search blueprints  
     * Filter by industry/compliance/price  
     * Checkout \+ download  
     * Dashboard to view earnings and blueprint performance

---

### **🧠 Code Instructions:**

* **Modular, reusable**, and **parameterized** functions only  
* Compatible with:  
  * **Bubble** (JavaScript plugins, API connectors)  
  * **Zapier’s MCP SDK** (as triggers/actions for blueprint syncs)  
  * **Node.js** or **serverless backends**  
* Each function should include:  
  * Purpose and inputs/outputs  
  * JSON schema  
  * Sample use cases

---

### **📦 Output Format:**

* Backend sample output:

```json
{
  "blueprintId": "abc123",
  "title": "E-commerce Content Flow",
  "description": "Automatically post new Shopify products to X and update inventory in QuickBooks.",
  "price": 15,
  "complianceTags": ["GDPR", "HIPAA"],
  "earnings": 11.25,
  "marketplaceFee": 3.75
}
```

*   
  Frontend output:  
  * Browsable cards, filters, pricing selectors  
  * Download tracking logic  
  * Earnings dashboard components (React or Bubble)

---

Use a real example:  
A creator uploads a “Notion-to-X content sync” blueprint for $15. The system autogenerates a GDPR tag, deducts 20% ($3), and displays it in the marketplace tagged under “Creator Tools.”

---

