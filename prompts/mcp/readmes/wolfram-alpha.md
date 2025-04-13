# wolfram-alpha MCP Server

Connect your chat repl to wolfram alpha computational intelligence

[What is an MCP Server?](https://www.anthropic.com/news/model-context-protocol)

| <!-- --> | <!-- --> |
|-----------|---------|
| **Image Source** | Official Image |
| **Author** | [SecretiveShell](https://github.com/SecretiveShell) |
| **Repository** | https://github.com/SecretiveShell/MCP-wolfram-alpha |
| **Dockerfile** | https://github.com/SecretiveShell/MCP-wolfram-alpha/blob/master/Dockerfile |
| **Docker Image built by** | Docker Inc. |
| **Licence** | MIT License |

## Tools Summary

 1. **`query-wolfram-alpha`**: Use Wolfram Alpha to answer a question. This tool should be used when you need complex math or symbolic intelligence.

## Tools

### Tool: **`query-wolfram-alpha`**

Use Wolfram Alpha to answer a question. This tool should be used when you need complex math or symbolic intelligence.

| Parameter | Type | Description |
| - | - | - |
| `query` | `string` |  |

## Use this MCP Server

```json
{
  "mcpServers": {
    "wolfram-alpha": {
      "command": "docker",
      "args": [
        "run",
        "-i",
        "--rm",
        "-e",
        "WOLFRAM_API_KEY",
        "mcp/wolfram-alpha"
      ],
      "env": {
        "WOLFRAM_API_KEY": "your-app-id"
      }
    }
  }
}
```

[Why is it safer to run MCP Servers with Docker?](https://www.docker.com/blog/the-model-context-protocol-simplifying-building-ai-apps-with-anthropic-claude-desktop-and-docker/)

## Rebuild this image

```console
docker build -t mcp/wolfram-alpha -f Dockerfile https://github.com/SecretiveShell/MCP-wolfram-alpha.git#master
```

