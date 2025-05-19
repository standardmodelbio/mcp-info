# mcp-info
MCP reference repo

## MCP documentation/info
### Issues:

250519 - was having tons of issues in getting a local MCP to work, essentially just follow the format as shown in the `./mcp.json` file 
- for MCPs that are on PyPI or other online public archive, can use uvx/bunx/etc
- for MCPs that are local, if in Python, be sure to use the following criteria

`
"command": "uv",
        "type": "stdio",
        "enable": true,
        "args": [
          "--directory {path to working directory} run {path from working dir to server file} {optional command to run the server if provided by script}"
        ]
`
