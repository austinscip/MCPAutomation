You are a senior software engineer experienced in building secure authentication and payment systems for SaaS platforms.

Build the full Auth & Payments Module for an AI-Powered MCP Automation Studio that supports user authentication and subscription payments. The module must include:

1\. User Authentication:  
   \- Sign-up, login, password reset flows.  
   \- OAuth 2.0 / social login integrations (Google, Facebook).  
   \- JWT-based session management with token refresh.  
   \- Role-based access control (e.g., admin, user, reseller).

2\. Subscription Payments:  
   \- Integration with Stripe or equivalent payment gateway.  
   \- Support multiple subscription tiers (Basic, Pro, Enterprise).  
   \- Handle billing cycles, trial periods, cancellations, and upgrades.  
   \- Webhooks to update user subscription status in real time.

3\. Security & Compliance:  
   \- Encrypt sensitive data (passwords, payment info).  
   \- Implement CSRF protection and rate limiting.  
   \- PCI DSS compliance considerations.

4\. User Management:  
   \- Admin dashboard to view/manage users and subscriptions.  
   \- API endpoints for account management.

Technical Implementation Requirements:

\- Structure all code as modular, reusable functions.  
\- Provide implementations compatible with:  
   \- Bubble (JavaScript plugins or API connectors)  
   \- Zapier MCP SDK (triggers, actions, searches)  
   \- Backend services (Node.js, serverless functions, or Express)  
\- Avoid hardcoding; use parameterized inputs.  
\- For each function, provide:  
   \- Purpose description  
   \- JSON schema for inputs  
   \- Example inputs and outputs  
\- Follow best security practices and provide code comments/documentation for maintainability.

Only provide code and documentation for this module. No unrelated content.