# MOTIONMAKER

Animates multi-part SketchUp models in the browser and records the result as video. Import a Collada export (or STL, OBJ, glTF), every group becomes a movable part, give parts moves, press play, record.

Conklin Office Furniture · Research and Development

## Run it

One file. Put `index.html` in a repo, turn on GitHub Pages, open it. It also runs from a double-click. three.js loads from cdn.jsdelivr.net, so it needs internet the first time.

DEMO BEAM loads the built-in POWER DREAM beam with its finished story: press PLAY.

## Export from SketchUp

File → Export → 3D Model → Collada (.dae), with:

- Preserve component hierarchies: on
- Triangulate all faces: on
- Export two-sided faces: off
- Export edges: off

Every top-level group or component comes in as one part. If a part should split further, PARTS → Split level → RE-SPLIT. If parts should be one, select them and MERGE SELECTED.

## Make an animation

1. **Click a part.** It turns amber. Its panel opens on the right.
2. **Give it a move.** Either drag the part in the view (shift drags on the floor), or pick a direction and distance under ADD A MOVE and press ADD. Each move starts where the part's last move ended, so the MOTION LIST reads like a script. Start time, duration and style are editable per move.
3. **Joints.** JOINTS gives a part a slide or hinge. The part's panel then shows a slider and ADD MOVE TO THIS VALUE. RIDES WITH attaches other parts (legs on a sleeve). LINK makes one joint copy another (both ends of a beam from one slider). Presets save joint values, for 48 / 54 / 60 / 72.
4. **Placements.** Move a part somewhere, SAVE it as a placement (FRONT, BACK, REMOVED). Clicking a placement adds a move to it.
5. **Timeline.** Every move is a bar. Drag bars to retime, click one to select it, scrub with the playhead.
6. **Camera and text.** CAMERA → frame the view → KEY CAMERA. TEXT → two lines, show and hide times.
7. **Record.** RECORD VIDEO → size and frame rate → downloads WebM, or MP4 in browsers that support it (Chrome 130+, Edge).

SAVE writes a `.mmk.json` project with the geometry inside, so it reopens without the source file.

## Keys

space play · ← → step a frame · F frame the selection · W / E move / rotate handles · del delete the selected move · esc deselect · ctrl+Z / ctrl+Y undo / redo
