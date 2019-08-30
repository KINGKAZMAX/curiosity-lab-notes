# Provide a complete path around the map

A new content and interaction exercise for making location information usable through a structured list. It proposes practical checks without claiming accessibility certification.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)
- [excalidraw/excalidraw — external upstream reference for a new exercise](https://github.com/excalidraw/excalidraw)

## Question

Can someone complete the main location task without understanding or manipulating a map? This exercise begins with the information a visitor needs: finding a place, checking its relevant details, and following an available action. It asks whether a list can provide an equally complete route through that information. The map remains one representation of the data, while the alternative must avoid becoming a reduced summary that hides essential attributes or available destinations.

## Design proposal

Propose a structured location list backed by the same records as the spatial view. Each entry should expose its name, location description, relevant category, and available action using ordinary document structure. Add search, predictable sorting, and clear result counts. Selection may synchronize the map, but list navigation must not depend on that synchronization. Announce changes in a restrained way and preserve focus when filters update the visible records.
