---
mcp:
  - container:
      image: mcp/filesystem:latest
      command:
        - .:
  - source:
      url: https://github.com/modelcontextprotocol/servers
---
