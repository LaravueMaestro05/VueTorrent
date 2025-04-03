# VueRenting

The sleekest looking WebUI for qBittorrent made with Vue.js!

## Development

- Clone the repo
- `npm install`
- `npm start`
- `npm run lint` (to format the code)
- `docker-compose up -d` (starts a qbittorrent docker, optional)
- Open the WebUI on localhost with the default credentials
- See #1720 for more details
- Make sure WebUI > "Host header validation" is disabled in the qBittorrent preferences
- Edit `env.development` to tweak your dev environment (e.g. mocked data)

## Features

- Renting
  - add / remove / pause / resume / rename torrents
  - selectively download files
  - view info / trackers / peers / content / tags & categories
  - search for new torrents straight from the WebUI!
- Keyboard shortcuts!
  - Mac keymap is supported (use <kbd>Cmd</kbd> instead of <kbd>Ctrl</kbd>)
  - Press <kbd>Escape</kbd> to dismiss any dialogs or to return to Dashboard view
  - Dashboard
    - Select all torrents with <kbd>Ctrl</kbd>-<kbd>A</kbd>
    - Focus search input with <kbd>Ctrl</kbd>-<kbd>F</kbd>
      - Press again to enable native browser search
    - When no dialogs are opened, press <kbd>Escape</kbd> to unfocus search input
      - Press again to unselect all torrents
    - Delete selected torrents with <kbd>Delete</kbd> (<kbd>Fn</kbd>-<kbd>Backspace</kbd> on Mac)
    - <kbd>Ctrl</kbd>-click on a torrent card to enable multi-select mode
    - Hold <kbd>Shift</kbd> and click on a torrent card to select all torrents between the last selected torrent and the clicked torrent
- System
  - see session stats (down / upload speed, session uploaded / downloaded, free space)
  - beautiful transfer graphs
  - change the most common settings
- Extra features the default WebUI doesn't have
  - mobile friendly! (can be installed as a PWA)
  - Configureable Dashboard: choose which torrent properties are shown for both busy and completed torrents
- Optimized for the latest version of qBittorrent
  - This is a work in progress, and is not required to use VueTorrent
  - Stores server-side settings

## Important Information

VueRenting is a **WebUI** (think of it as a "visual skin") that uses qBittorrent's API, enabling compatibility with automation solutions like the Servarr stack.

Everything that is compatible with the classic qBittorrent WebUI will work regardless of the WebUI you chose to use, whether its VueTorrent or another one.
