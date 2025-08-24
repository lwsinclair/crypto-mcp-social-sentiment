[![MSeeP.ai Security Assessment Badge](https://mseep.net/pr/hive-intel-crypto-mcp-social-sentiment-badge.png)](https://mseep.ai/app/hive-intel-crypto-mcp-social-sentiment)

# Hive MCP Social Sentiment

## Overview
Model Context Protocol (MCP) server for cryptocurrency social sentiment analysis and community metrics. This MCP provides comprehensive tools for analyzing social media sentiment, community engagement, and market sentiment across various platforms and blockchain projects.

## Connection Details
- **Transport**: HTTP (Remote only)
- **URL**: `https://mcp.hiveintelligence.xyz/hive_social_sentiment/mcp`
- **Protocol**: Model Context Protocol (MCP)

## Features
- Social media sentiment analysis
- Community growth tracking
- Influencer activity monitoring
- Trending topics and hashtags
- Project mention tracking
- Sentiment score calculations
- Community engagement metrics
- Social volume analysis
- FUD and FOMO detection
- Whale alert integration
- News sentiment aggregation
- Cross-platform analytics

## Usage

### Claude Desktop Configuration
Add to your Claude Desktop configuration file:

```json
{
  "mcpServers": {
    "hive-social-sentiment": {
      "url": "https://mcp.hiveintelligence.xyz/hive_social_sentiment/mcp",
      "transport": "http"
    }
  }
}
```

### MCP Client Integration
```javascript
import { Client } from '@modelcontextprotocol/sdk';

const client = new Client({
  name: 'social-sentiment-client',
  version: '1.0.0'
});

await client.connect({
  url: 'https://mcp.hiveintelligence.xyz/hive_social_sentiment/mcp',
  transport: 'http'
});
```

## Available Tools

### `analyze_sentiment`
Analyze sentiment for specific tokens or projects
```json
{
  "tool": "analyze_sentiment",
  "params": {
    "tokens": ["BTC", "ETH", "SOL"],
    "timeframe": "24h",
    "platforms": ["twitter", "reddit", "telegram"]
  }
}
```

### `track_community_growth`
Monitor community growth metrics
```json
{
  "tool": "track_community_growth",
  "params": {
    "project": "ethereum",
    "metrics": ["followers", "active_users", "engagement_rate"],
    "period": "30d"
  }
}
```

### `monitor_influencers`
Track influencer activity and impact
```json
{
  "tool": "monitor_influencers",
  "params": {
    "category": "crypto",
    "min_followers": 10000,
    "sentiment_filter": "bullish"
  }
}
```

### `detect_trends`
Identify trending topics and narratives
```json
{
  "tool": "detect_trends",
  "params": {
    "timeframe": "6h",
    "min_mentions": 100,
    "categories": ["defi", "nft", "layer2"]
  }
}
```

### `measure_fud_fomo`
Measure FUD and FOMO levels
```json
{
  "tool": "measure_fud_fomo",
  "params": {
    "tokens": ["BTC", "ETH"],
    "sensitivity": "high",
    "include_metrics": true
  }
}
```

## Keywords
social sentiment, sentiment analysis, community metrics, social media analytics, crypto sentiment, community growth, influencer tracking, trending topics, social volume, engagement metrics, FUD detection, FOMO analysis, market sentiment, social signals, community analytics, Twitter sentiment, Reddit analysis, Telegram monitoring, Discord metrics, MCP, Model Context Protocol, Web3 social, HTTP MCP server, remote MCP, Hive Intelligence, crypto social media, sentiment scoring, narrative tracking

## License
MIT

## Support
For issues and feature requests, please open an issue on GitHub.

## About Hive Intelligence
Part of the Hive Intelligence suite of blockchain analytics MCP servers.