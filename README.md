# Haridev's Brain

A node-link graph view built with [D3.js](https://d3js.org/), running a force-directed graph layout heavily inspired by Obsidian's graph view — I'm a heavy Obsidian user, so this is basically that idea pulled out onto the web.

**Live:** https://harideviitg.github.io/mindmap/

## How it's structured

Everything starts from the center node, "Haridev's Brain" — that's where the thoughts emerge from. From there it branches out into a handful of top-level nodes (right now: Principles, Process, Influences, and Still Thinking).

The number of branches isn't fixed and might change month to month. If a person's thoughts and opinions never change, what kind of person is that, honestly.

Each of those branches fans out further into the specific ideas underneath it, so the hierarchy reads: **brain → square → triangle.**

There's also an "About" node sitting next to the top-level branches. It explains what this view is, how to tweak the layout using the controls panel, and a disclaimer that the content here is a living thing and will keep getting updated.

## Interacting with it

- Click any node to open a reader-style sidebar with the full text for that node.
- Drag any node to reposition it — the simulation reacts live.
- Use the "Show controls" panel (bottom-left) to tune the force simulation: center force, repel force, link force/distance, text fade threshold, node size, and link thickness.
- Hit the reset icon to clear any dragging and snap everything back to its default layout.

## Stack

Single static `index.html` — D3.js (force simulation + zoom/drag), no build step, no framework. Deployed straight off the `main` branch via GitHub Pages.
