# MDict MCP Server


Available Tools: [TOOLS.md](./TOOLS.md)


Dependencies: 

- mcp
- mdict-utils


Claude Desktop

![Claude Desktop](./claude.png)

```json
{
  "mcpServers": {
    "mdict": {
      "command": "uvx",
      "args": [
        "mdict-mcp"
      ],
      "env": {
        "MDICT_DICTIONARY_DIR": "/path/to/mdicts/"
      }
    }
  }
}
```

ChatWise

![ChatWise](./chatwise.png)

```bash
# type stdio
# env MDICT_DICTIONARY_DIR=/path/to/mdicts/
uvx mdict-mcp
```

Local testing:

```bash
uv --directory $HOME/Developer/mdict-mcp run mdict-mcp
```
