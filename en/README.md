# Boat race

This English project builds a Scratch boat-racing game in the Raspberry Pi Code Editor.

## Project files

- `landing.md` introduces the game and embeds the published Scratch player.
- `step_1.md` to `step_13.md` contain 12 build steps and an optional challenge.
- `meta.yml` defines the step titles, order, completion markers and landing-page setting.
- `code/editor-boat-race-starter/` contains `editor-boat-race-starter.sb3`, with the boat and two race-course backdrops but no scripts, variables or lists.
- `code/editor-boat-race-complete/` contains `editor-boat-race-complete.sb3`, with movement, collisions, a visible timer, boosters and a spinning gate.
- Both code folders have a `project_config.yml` with a matching identifier, `type: 'code_editor_scratch'` and `build: true`.
- `resources/BoatRaceResources.sb3` is the downloadable copy of the editor starter.
- `solutions/BoatRace-Finished.sb3` is the downloadable copy of the complete project.
- `images/` contains the project banner, screenshots and sprite thumbnails. The repository's `banner.png` is a copy of `images/small_banner.png`.

## Metadata

The project uses `landing: true` and `pdf: false`. Completion markers are on step 2 (`engaged`), step 8 (`internal`) and step 12 (`external`). Step 13 has `challenge: true` and no completion marker.

Keep the metadata titles and order in sync with the numbered step files. Update `last_tested` after testing the finished game.

## Updating the Scratch files

Keep each editor archive and its downloadable copy identical. The starter should leave learners to create their own scripts and variables. The complete project should match the lesson, including two-second crash and winning messages and a visible `time` monitor.

After publication, check that both editor projects load as Scratch and that the landing-page game plays correctly.
