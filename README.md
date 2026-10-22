# Onlineprinters

Find and configure print products from Onlineprinters (flyers, business cards, posters, banners, stickers, cards, brochures), see the shop's list price and estimated delivery date, check whether a print file fits, and open the configured product in the Onlineprinters shop.

## What is in this plugin

- A connector that points to the public Onlineprinters MCP server at https://mcp.onlineprinters.com/claude/mcp. No sign-in and no key are needed.
- A skill, print-advice, that tells Claude how to use the tools: pick the shop of the delivery country first, quote only the prices the tools return, and end with the shop link.

## How to use it

Add the plugin, then ask in everyday words, for example: "I need 500 A5 flyers for our summer party in Nuremberg. What do they cost, when would they arrive, and where can I order them?" Adding a plugin does not add its connector to your account: open the plugin under Customize > Plugins, select its Connectors tab and connect it, then allow its tools when Claude asks.

## What it sends

The plugin is read-only. It sends the tool requests Claude makes (search words, chosen options, quantities, delivery country, file dimensions, shop links you paste) to the server above, which Onlineprinters GmbH operates. The server asks Onlineprinters' own product catalogue service for the answer. The hosting service also records technical connection data such as the IP address of the calling system (in Claude Code, your own public IP address) and uses it to limit the number of requests per caller. The plugin runs no local code and reads no files or credentials from your computer. Please leave names, addresses and payment data out of your questions: the plugin does not need them.

## Limits

No ordering, payment, file upload, order status or invoices: basket, vouchers, upload, payment and the order stay in the Onlineprinters shop. No login is needed. Shops (German-language): Germany, Austria, Switzerland (CHF), Luxembourg and Italy (South Tyrol). Prices are list prices before vouchers; shipping costs and the binding price are shown in the shop basket. Delivery dates are estimates.

## Install

In the Claude apps and in Claude Code, add it from the plugin directory. In Claude Code you can also install it from its marketplace:

```
/plugin install onlineprinters --marketplace onlineprinters-ai/onlineprinters-claude-plugin
```

## Licence

Apache License 2.0, see LICENSE. The Onlineprinters name and logo are trademarks of Onlineprinters GmbH and are not licensed under it.

## Privacy and support

Privacy notice: https://privacy-policy-url-placeholder.invalid/
Help and support: https://support-url-placeholder.invalid/
