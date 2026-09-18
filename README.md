# MOTIONMAKER

CONKLIN OFFICE FURNITURE - RESEARCH AND DEVELOPMENT

Part animation for SketchUp models. Import a Collada export (or STL, OBJ, glTF), every group becomes a movable part, give parts moves on a timeline, and record the result as video. Built for product concept clips like the expandable POWER DREAM beam.

OUTPUT IN WEBM AND MP4 VIDEO, MMK PROJECT FILE

LAUNCH — https://wesprojects.github.io/MOTIONMAKER

---

## START

Open the launch link. DEMO BEAM loads the built-in POWER DREAM beam with its finished story: press PLAY. IMPORT MODEL opens your own file.

## EXPORT FROM SKETCHUP

File → Export → 3D Model → Collada (.dae)

- Preserve component hierarchies: on
- Triangulate all faces: on
- Export two-sided faces: off
- Export edges: off

Every top-level group or component comes in as one part. PARTS → Split level → RE-SPLIT breaks parts down further. MERGE SELECTED fuses parts into one.

## MAKE AN ANIMATION

1. **Click a part.** It turns amber and its panel opens on the right.
2. **Give it a move.** Drag the part in the view (shift drags on the floor), or pick a direction and distance under ADD A MOVE. Each move starts where the last one ended, so the MOTION LIST reads like a script. Start, duration and style are editable per move.
3. **Joints.** JOINTS gives a part a slide or hinge. The part's panel then shows a slider and ADD MOVE TO THIS VALUE. RIDES WITH attaches other parts (legs on a sleeve). LINK makes one joint follow another. Presets save joint values (48 / 54 / 60 / 72).
4. **Placements.** Move a part, SAVE the spot as a placement (FRONT, BACK, REMOVED). Clicking a placement adds a move to it.
5. **Timeline.** Every move is a bar. Drag to retime, click to select, scrub with the playhead.
6. **Camera and text.** CAMERA → frame the view → KEY CAMERA. TEXT → two lines with show and hide times.
7. **Record.** RECORD VIDEO → size and frame rate. WebM everywhere, MP4 where the browser supports it (Chrome 130+, Edge).

SAVE writes a `.mmk.json` project with the geometry inside, so it reopens without the source file.

## KEYS

space play · ← → step a frame · F frame the selection · W / E move / rotate handles · del delete the selected move · esc deselect · ctrl+Z / ctrl+Y undo / redo
