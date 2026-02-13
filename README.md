MCPs disabled globally, enable them in project `opencode.json`:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "mcp": {
    "figma": {
      "enabled": true,
      "type": "remote",
      "url": "http://127.0.0.1:3845/sse"
    },
    "apollo": {
      "enabled": true,
      "type": "remote",
      "url": "https://mcp.apollographql.com"
    },
    "code-index": {
      "enabled": true,
      "type": "local",
      "command": [
        "uvx",
        "code-index-mcp",
        "--project-path",
        "/Users/carloscoves/projects/LECNebulaApp"
      ]
    }
  }
}
```
