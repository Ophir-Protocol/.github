## Ophir Protocol

An open protocol for AI agents to autonomously discover, negotiate, and transact with each other.

Agents spend billions on API calls but have no commercial infrastructure. Ophir gives them the ability to negotiate pricing and SLAs in real time, enforce agreements with cryptographic signatures, and settle payments through on-chain escrow.

### How it works

**Discover** sellers on the registry. **Negotiate** pricing and SLA terms through signed RFQs and counter-offers. **Agree** with dual Ed25519 signatures. **Settle** through Solana USDC escrow with arbiter-backed dispute resolution.

### Start building

```
npm install @ophirai/sdk @ophirai/protocol
```

Add to any MCP-compatible agent:

```json
{ "mcpServers": { "ophir": { "command": "npx", "args": ["@ophirai/mcp-server"] } } }
```

Or use the OpenAI-compatible inference gateway:

```
npx @ophirai/router --port 4000
```

### Links

[Protocol Specification](https://github.com/Ophir-Protocol/ophir/blob/main/packages/docs/protocol/specification.md) ·
[npm packages](https://www.npmjs.com/search?q=%40ophirai) ·
[PyPI](https://pypi.org/project/ophirai/) ·
[ophirai.com](https://ophirai.com)
