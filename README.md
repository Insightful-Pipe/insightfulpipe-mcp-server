# InsightfulPipe MCP Server

[![MCP Compatible](https://img.shields.io/badge/MCP-Compatible-blue)](https://insightfulpipe.com/mcp-servers/insightfulpipe)
[![Insightful Pipe](https://img.shields.io/badge/Insightful_Pipe-MCP_Servers-purple)](https://insightfulpipe.com/mcp-servers)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **One MCP server for every marketing, SEO, e-commerce and data source connected to your InsightfulPipe workspace.**

The all-in-one server from the [Insightful Pipe MCP Server Collection](https://insightfulpipe.com/mcp-servers) — use every connected platform from Claude, ChatGPT, Cursor, and other AI assistants through the Model Context Protocol (MCP).

<img src="images/insightfulpipe-icon.svg" alt="InsightfulPipe MCP Server" width="64" height="64">

## MCP Server URL

```
https://main.insightfulmcp.com/
```

## What is InsightfulPipe MCP?

InsightfulPipe MCP is a **remote Model Context Protocol server** that gives AI assistants one connection to every data source in your InsightfulPipe workspace. Access all your connected data sources through a single unified interface for comprehensive analytics.

## Installation

### Claude

1. Copy the MCP Server URL: `https://main.insightfulmcp.com/`
2. Open [Claude Connectors Settings](https://claude.ai/settings/connectors)
3. Scroll to the bottom and click **Add custom connector**
4. Paste the URL and click **Add**
5. Click **Connect** on the connector to start authorization
6. Click **Authorize access** in the browser to complete the connection

### ChatGPT

Custom MCP servers are added through ChatGPT's **Developer mode**. Availability depends on your ChatGPT plan, and workspace admins may need to allow it.

1. Turn on **Developer mode** in ChatGPT settings
2. Create a new app for a remote MCP server and paste the URL: `https://main.insightfulmcp.com/`
3. Authorize with your InsightfulPipe account

See OpenAI's guide: [Developer mode and MCP apps in ChatGPT](https://help.openai.com/en/articles/12584461-developer-mode-and-mcp-apps-in-chatgpt)

### Claude Code

```bash
claude mcp add --transport http insightfulpipe https://main.insightfulmcp.com/
```

### Cursor

Add the server to `~/.cursor/mcp.json` (all projects) or `.cursor/mcp.json` (one project):

```json
{
  "mcpServers": {
    "insightfulpipe": {
      "url": "https://main.insightfulmcp.com/"
    }
  }
}
```

Then authorize the connection when Cursor prompts you.

## Available Tools

| Tool | Description |
|------|-------------|
| `list_platforms` | List every supported platform with a short description |
| `query_contexts` | Discover connected accounts, available actions, and the exact request format for a platform |
| `query_data` | Run read-only queries such as reports, analytics, and listings |
| `execute_action` | Run write operations such as create, update, and publish |
| `prompts_menu` | Browse ready-to-use prompts |

## Dedicated MCP Servers

Prefer one platform per connection? Every platform also has its own server:

- [Ads Libraries](https://github.com/Insightful-Pipe/ads-libraries-mcp-server)
- [Airtable](https://github.com/Insightful-Pipe/airtable-mcp-server)
- [BigQuery](https://github.com/Insightful-Pipe/bigquery-mcp-server)
- [Bing Webmaster Tools](https://github.com/Insightful-Pipe/bing-webmaster-mcp-server)
- [CallRail](https://github.com/Insightful-Pipe/callrail-mcp-server)
- [DataForSEO](https://github.com/Insightful-Pipe/dataforseo-mcp-server)
- [Enrichment Crawlers](https://github.com/Insightful-Pipe/enrichment-mcp-server)
- [Facebook Ads](https://github.com/Insightful-Pipe/facebook-ads-mcp-server)
- [Facebook Pages](https://github.com/Insightful-Pipe/facebook-pages-mcp-server)
- [Google Ads](https://github.com/Insightful-Pipe/google-ads-mcp-server)
- [Google Analytics 4](https://github.com/Insightful-Pipe/google-analytics-mcp-server)
- [Google Merchant Center](https://github.com/Insightful-Pipe/google-merchant-center-mcp-server)
- [Google My Business](https://github.com/Insightful-Pipe/google-my-business-mcp-server)
- [Google Search Console](https://github.com/Insightful-Pipe/google-search-console-mcp-server)
- [Google Sheets](https://github.com/Insightful-Pipe/google-sheets-mcp-server)
- [Google Tag Manager](https://github.com/Insightful-Pipe/google-tag-manager-mcp-server)
- [Instagram Analytics](https://github.com/Insightful-Pipe/instagram-mcp-server)
- [Klaviyo](https://github.com/Insightful-Pipe/klaviyo-mcp-server)
- [LinkedIn Ads](https://github.com/Insightful-Pipe/linkedin-ads-mcp-server)
- [LinkedIn Page & Profile](https://github.com/Insightful-Pipe/linkedin-pages-mcp-server)
- [Magento](https://github.com/Insightful-Pipe/magento-mcp-server)
- [Mailchimp](https://github.com/Insightful-Pipe/mailchimp-mcp-server)
- [Microsoft Ads](https://github.com/Insightful-Pipe/microsoft-ads-mcp-server)
- [Microsoft Clarity](https://github.com/Insightful-Pipe/microsoft-clarity-mcp-server)
- [MySQL](https://github.com/Insightful-Pipe/mysql-mcp-server)
- [Notion](https://github.com/Insightful-Pipe/notion-mcp-server)
- [OpenAI Ads](https://github.com/Insightful-Pipe/openai-ads-mcp-server)
- [PageSpeed Insights](https://github.com/Insightful-Pipe/pagespeed-mcp-server)
- [Pinterest Ads](https://github.com/Insightful-Pipe/pinterest-ads-mcp-server)
- [Pinterest Pages](https://github.com/Insightful-Pipe/pinterest-pages-mcp-server)
- [PostgreSQL](https://github.com/Insightful-Pipe/postgresql-mcp-server)
- [SQL Server](https://github.com/Insightful-Pipe/mssql-mcp-server)
- [Screenshots](https://github.com/Insightful-Pipe/screenshot-mcp-server)
- [Shopify](https://github.com/Insightful-Pipe/shopify-mcp-server)
- [Slack](https://github.com/Insightful-Pipe/slack-mcp-server)
- [Snapchat Ads](https://github.com/Insightful-Pipe/snapchat-ads-mcp-server)
- [Stripe](https://github.com/Insightful-Pipe/stripe-mcp-server)
- [Telegram](https://github.com/Insightful-Pipe/telegram-mcp-server)
- [TikTok Ads](https://github.com/Insightful-Pipe/tiktok-ads-mcp-server)
- [TikTok Pages](https://github.com/Insightful-Pipe/tiktok-pages-mcp-server)
- [Web Crawler](https://github.com/Insightful-Pipe/web-crawler-mcp-server)
- [WooCommerce](https://github.com/Insightful-Pipe/woocommerce-mcp-server)
- [WordPress](https://github.com/Insightful-Pipe/wordpress-mcp-server)
- [X Ads](https://github.com/Insightful-Pipe/x-ads-mcp-server)
- [YouTube Analytics](https://github.com/Insightful-Pipe/youtube-mcp-server)

## Usage Examples

```
"Compare my Google Ads and Meta Ads spend and ROAS for the last 30 days"
```

```
"Which pages get the most organic clicks in Search Console, and how do they convert in GA4?"
```

```
"List every data source connected to my workspace"
```

## Explore More MCP Servers by Insightful Pipe

Visit **[insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)** to discover our full collection of MCP servers.

- [Google Ads MCP](https://insightfulpipe.com/mcp-servers/google-ads)
- [Meta Ads MCP](https://insightfulpipe.com/mcp-servers/facebook-ads)
- [Google Analytics MCP](https://insightfulpipe.com/mcp-servers/google-analytics)
- [Google Search Console MCP](https://insightfulpipe.com/mcp-servers/google-search-console)

**[View All MCP Servers →](https://insightfulpipe.com/mcp-servers)**

## Resources

- [Documentation](https://insightfulpipe.com/docs)
- [Video Tutorial](https://www.youtube.com/playlist?list=PLJNzvjxzI5Xwe__BJJLAelSF0ewO3mEFk)
- [InsightfulPipe Blog](https://insightfulpipe.com/blog)

## Support

- **Documentation**: [insightfulpipe.com/docs](https://insightfulpipe.com/docs)
- **All MCP Servers**: [insightfulpipe.com/mcp-servers](https://insightfulpipe.com/mcp-servers)
- **Email**: support@insightfulpipe.com

---

**[Insightful Pipe](https://insightfulpipe.com)** — AI-powered marketing analytics through MCP servers. [Explore all integrations →](https://insightfulpipe.com/mcp-servers)

## License

MIT License - see [LICENSE](LICENSE) for details.
