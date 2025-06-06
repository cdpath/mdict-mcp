# MDict MCP Server

![Claude Desktop](./claude.png)


Available Tools: [TOOLS.md](./TOOLS.md)


Dependencies: 

- mcp
- mdict-utils


Configs:

<table>
<tr>
<td> Client </td> <td> Config </td>
</tr>
<tr>
<td> Claude Desktop </td>
<td>

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

<tr>
<td> ChatWise </td>
<td>

```bash
# type stdio
# env MDICT_DICTIONARY_DIR=/path/to/mdicts/
uvx mdict-mcp
```
</td>
</tr>
</table>

Local testing:

```bash
uv --directory $HOME/Developer/mdict-mcp run mdict-mcp
```
