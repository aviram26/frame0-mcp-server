[![smithery badge](https://smithery.ai/badge/@niklauslee/frame0-mcp-server)](https://smithery.ai/server/@niklauslee/frame0-mcp-server)

[![Frame0 MCP Video Example](https://github.com/niklauslee/frame0-mcp-server/raw/main/thumbnail.png)](https://frame0.app/videos/frame0-mcp-example.mp4)

# Muzika Frame0 MCP Server

[Frame0](https://frame0.app/) is a Balsamiq-alternative wireframe tool for modern apps. **Muzika Frame0 MCP Server** is a customized version that allows you to create and modify wireframes in Frame0 specifically for the Muzika music analytics project.

## About Muzika Project

Muzika is a comprehensive music band and artist data management system designed to capture and analyze complex relationships in the music industry:

- **Artist career paths**: Track artists moving between bands
- **Temporal relationships**: When artists were in which bands  
- **Cross-band connections**: Find artists who played together
- **Career timeline analysis**: Complete artist journey visualization

## Setup

Prerequisite:
- [Frame0](https://frame0.app/) `v1.0.0-beta.17` or higher.
- [Node.js](https://nodejs.org/) `v22` or higher.

Setup for Claude Desktop in `claude_desktop_config.json` as below:

```json
{
  "mcpServers": {
    "muzika-frame0-mcp-server": {
      "command": "npx",
      "args": ["-y", "muzika-frame0-mcp-server"]
    }
  }
}
```

You can use `--api-port=<port>` optional parameter to use another port number for Frame0's API server.

## Music Analytics Wireframe Examples

- _"Create a music analytics dashboard for Desktop in Frame0"_
- _"Create an artist career timeline visualization for Tablet in Frame0"_
- _"Create a band member relationship diagram for Desktop in Frame0"_
- _"Create a music project timeline for Phone in Frame0"_
- _"Add a cross-band connection visualization"_
- _"Create a music genre analytics chart"_
- _"Design a music industry network graph"_

## Available Tools

### Basic Frame0 Tools
- `create_frame`
- `create_rectangle`
- `create_ellipse`
- `create_text`
- `create_line`
- `create_polygon`
- `create_connector`
- `create_icon`
- `create_image`
- `update_shape`
- `duplicate_shape`
- `delete_shape`
- `search_icons`
- `move_shape`
- `align_shapes`
- `group`
- `ungroup`
- `set_link`
- `export_shape_as_image`
- `add_page`
- `update_page`
- `duplicate_page`
- `delete_page`
- `get_current_page_id`
- `set_current_page_by_id`
- `get_page`
- `get_all_pages`
- `export_page_as_image`

### Music-Specific Tools (Coming Soon)
- `create_music_dashboard`
- `create_artist_timeline`
- `create_band_relationship_diagram`
- `create_music_analytics_chart`
- `create_cross_band_connections`

## Development

1. Clone this repository.
2. Build with `npm run build`.
3. Update `claude_desktop_config.json` in Claude Desktop as below.
4. Restart Claude Desktop.

```json
{
  "mcpServers": {
    "muzika-frame0-mcp-server": {
      "command": "node",
      "args": ["<full-path-to>/muzika-frame0-mcp-server/build/index.js"]
    }
  }
}
```

## Music Analytics Use Cases

This MCP server is specifically designed to help create wireframes for:

1. **Artist Career Dashboards**: Visualize artist career paths and transitions
2. **Band Relationship Networks**: Show connections between bands and artists
3. **Temporal Analytics**: Timeline-based visualizations of music industry data
4. **Cross-Band Analysis**: Identify artists who played in multiple bands
5. **Music Project Tracking**: Album and project timeline visualizations

## Contributing

This is a fork of the original [frame0-mcp-server](https://github.com/niklauslee/frame0-mcp-server) by [@niklauslee](https://github.com/niklauslee), customized for the Muzika music analytics project.

## License

MIT License - see LICENSE file for details.
