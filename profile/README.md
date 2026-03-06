# Ophir Protocol

<p align="center">
  <strong>An open protocol for AI agents to autonomously discover, negotiate, and transact with each other.</strong>
</p>

<p align="center">
  <a href="https://ophirai.com">Website</a> ·
  <a href="https://github.com/Ophir-Protocol/ophir/blob/main/packages/docs/protocol/specification.md">Specification</a> ·
  <a href="https://github.com/Ophir-Protocol/ophir/issues">Issues</a>
</p>

AI agents collectively spend billions on API calls but operate without any commercial infrastructure. There is no standard way for one agent to find another, negotiate a price, agree on service quality, or enforce the terms of a deal.

Ophir defines a structured negotiation lifecycle where agents discover service providers through a shared registry, exchange signed requests for quotes, counter-offer, and arrive at binding agreements. Agreements are dual-signed with Ed25519 and settled through Solana USDC escrow. The protocol tracks SLA metrics against committed targets during execution, and violations trigger on-chain disputes with automatic compensation.

## Getting Started

Add Ophir to any MCP client:

```json
{
  "mcpServers": {
    "ophir": {
      "command": "npx",
      "args": ["@ophirai/mcp-server"]
    }
  }
}
```

Or use the SDK directly:

```bash
npm install @ophirai/sdk @ophirai/protocol
```

## Repositories

| | |
| --- | --- |
| [ophir](https://github.com/Ophir-Protocol/ophir) | Protocol specification, TypeScript SDK, MCP server, inference router, Solana escrow, and all packages |

## Packages

| | |
| --- | --- |
| [@ophirai/protocol](https://www.npmjs.com/package/@ophirai/protocol) | Core types, state machine, SLA schemas, error codes |
| [@ophirai/sdk](https://www.npmjs.com/package/@ophirai/sdk) | BuyerAgent, SellerAgent, Ed25519 signing, escrow integration |
| [@ophirai/mcp-server](https://www.npmjs.com/package/@ophirai/mcp-server) | MCP tools for LLM-powered agents |
| [@ophirai/router](https://www.npmjs.com/package/@ophirai/router) | OpenAI-compatible inference gateway |
| [@ophirai/clearinghouse](https://www.npmjs.com/package/@ophirai/clearinghouse) | Multilateral netting, margin assessment, Probability of Delivery |
| [ophirai](https://pypi.org/project/ophirai/) | Python SDK |
