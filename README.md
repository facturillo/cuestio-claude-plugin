# Cuestio

Ask Claude about the prices Panama's online stores publish. Cuestio keeps those prices, read every day, product by product and store by store, and its Price Radar gives an organization a view of them. This plugin connects Claude to your organization's Price Radar and teaches it how to answer questions about store prices. Questions about prices only read, and the tools that add or change something are described under Data.

## Use it

Install the plugin, then connect the Cuestio connector from the plugin's Connectors tab. Claude opens the Cuestio dashboard at app.cuestio.com, where you sign in and approve the connection with the same account you use there. Then ask in Spanish or English:

- "What do the online supermarkets list for a 425 g jar of instant coffee, and which store is cheapest today?"
- "Which products on our watch list changed price this week, and by how much?"
- "Compare this basket of ten products across the stores."
- "How does our store's index compare with our two main competitors this month?"
- "Which promotions do the stores publish in beverages?"

The `ask-the-price-radar` skill tells Claude which Cuestio tool answers which question (product search, current offers, price history, a basket compared across stores, price changes, promotions, availability, the price index and the stores covered), how to handle the watch list, baskets and exports, and how to say prices.

## What it needs

A Cuestio account that belongs to an organization with the Price Radar active. An admin of the organization invites you and decides who can see it. Baskets also need a facturillo account. A tool that does not apply to the account says so plainly.

## Data

The plugin sends nothing on its own. Every question Claude answers goes through the Cuestio connector at `mcp.cuestio.com`, which reads the online prices of the products and stores you ask about. It reads nothing else of your organization. When you ask Claude to, the connector also changes things: it keeps your organization's shared watch list of up to 5,000 products, which the members of the organization share, and it writes a CSV file of a price report on Cuestio's server behind a private link that expires after 15 minutes. The file is deleted after a day. If you also have a facturillo account, it creates, changes and deletes the baskets you see in the facturillo app. The prices are the ones the stores publish on their own online shops, read daily. These are online listings and prices, never sales, units sold or market shares. The connector is operated by facturillo Inc.

## Privacy policy

https://facturillo.com/privacy (English: https://facturillo.com/en/privacy). The section "AI Assistant Connections (facturillo AI Connector)" and its part "Cuestio: the organization dashboard and its Price Radar connection" cover the Cuestio connector this plugin uses: who can connect, what the assistant can reach, what is recorded and how to disconnect.

## Support

info@facturillo.com · Documentation: https://cuestio.com/ai/
