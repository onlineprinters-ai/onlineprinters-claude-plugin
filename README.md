# Onlineprinters

Find and configure print products from Onlineprinters (flyers, business cards, posters, banners, stickers, cards, brochures), see the shop's list price and estimated delivery date, check whether a print file fits, and open the configured product in the Onlineprinters shop or put it into the shop basket with one click through a cart link. After you connect your Onlineprinters customer account, see your own orders, invoices and quotes.

## What is in this plugin

- A connector that points to the public Onlineprinters MCP server at https://mcp.onlineprinters.com/claude/mcp. The catalogue tools answer without signing in and without a key; the four account tools ask you to connect your Onlineprinters customer account once. If you have no account yet, you register in the shop while connecting. Connecting the customer account works in the Claude apps; Claude Code cannot connect it yet and uses the catalogue tools only.
- A skill, print-advice, that tells Claude how to use the tools: pick the shop of the delivery country first, quote only the prices the tools return, and end with the shop link and the cart link.

## How to use it

Add the plugin, then ask in everyday words, for example: "I need 500 A5 flyers for our summer party in Nuremberg. What do they cost, when would they arrive, and where can I order them?" Adding a plugin does not add its connector to your account: open the plugin under Customize > Plugins, select its Connectors tab and connect it, then allow its tools when Claude asks.

## What it sends

The plugin is read-only. It sends the tool requests Claude makes (search words, chosen options, quantities, delivery country, file dimensions, shop links you paste) to the server above, which Onlineprinters GmbH operates. The server asks Onlineprinters' own product catalogue service for the answer. The hosting service also records technical connection data such as the IP address of the calling system (in Claude Code, your own public IP address) and uses it to limit the number of requests per caller; the server also limits the calls of the account tools per customer account. The plugin runs no local code and reads no files or credentials from your computer. Please leave names, addresses and payment data out of your questions: the plugin does not need them.

After you connect your Onlineprinters customer account (you sign in to the shop and choose the permissions for orders, invoices and quotes), the server reads only the parts you allowed, to answer your questions about them; addresses, contact and payment data are removed before an answer goes to Claude. Your shop login is stored encrypted for the connection and deleted when you disconnect (each account answer has a disconnect link) or after 90 days without use.

## Limits

No ordering, payment or file upload, and nothing in your customer account is changed (no cancelling, no reordering): basket, vouchers, upload, payment and the order stay in the Onlineprinters shop; a cart link fills the shop basket only when you click it. Shops (German-language): Germany, Austria, Switzerland (CHF), Luxembourg and Italy (South Tyrol); Business shops (Pro) and brand shops are not included. Some promotional items, such as pocket knives, multitools and lighters, are not available through the plugin. Prices are list prices before vouchers; shipping costs and the binding price are shown in the shop basket. Delivery dates are estimates.

## Install

In the Claude apps and in Claude Code, add it from the plugin directory.

## Licence

Apache License 2.0, see LICENSE. The Onlineprinters name and logo are trademarks of Onlineprinters GmbH and are not licensed under it.

## Privacy and support

Privacy notice: https://www.onlineprinters.org/c/about-us/legal-information/ai-connector/privacy-ai-connector
Help and support: https://www.onlineprinters.org/c/faq/ai-plugin-claude
