# ParalivesBuddy

Working concept repo for a first Paralives mod and the pipeline around it.

## Goal

Build a small, safe test mod first, prove we can package it locally on Windows, then publish it through the game's Steam Workshop flow.

## Important note

For mods, the destination is usually **Steam Workshop**, not the regular Steam Store. The Steam Store is for games, DLC, and other store products. Workshop is the place where players subscribe to and download mods.

## Phase 1: Simple test mod

Start with the least risky mod possible:

1. Pick one tiny, visible change.
2. Keep it easy to revert.
3. Make sure it does not depend on complex game systems.

Good first examples:

1. A cosmetic tuning change.
2. A small object or item tweak.
3. A simple replacement asset or data edit.

The best first mod is the one that proves the toolchain without causing gameplay regressions.

## Phase 2: Windows build flow

On the Windows machine, the goal is to get a repeatable loop:

1. Open the mod project.
2. Make a small change.
3. Build/package the mod.
4. Install or load it in the game.
5. Verify it appears in-game.

If the game provides an editor or mod tools, we should use those as the primary path. If not, we should document the file structure and any manual packaging steps here.

## Phase 3: Workshop publish flow

Once the test mod works locally:

1. Create or open the Steam Workshop item.
2. Upload the packaged mod.
3. Add a preview image and clear description.
4. Tag it correctly.
5. Subscribe to it from a clean test account or test install.
6. Confirm the Workshop version updates correctly after a change.

## What we still need to figure out

1. What file format Paralives expects for mods.
2. Whether the game uses an editor, a packager, or both.
3. How the mod folder should be structured on Windows.
4. Whether the first upload path is direct from the game or through a separate tool.

## Working approach

We should keep the first target boring and reliable:

1. Make one tiny mod.
2. Make one clean build.
3. Make one Workshop upload.
4. Only then start building bigger, bolder mod ideas.
