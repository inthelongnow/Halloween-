# Pipeline pack

Small pack pointed at the creature types already in play. Same scaffold every time: black void, liquid glass, false-color neon, radial sacred geometry, glitch as structure. The twist is the organism.

Toolchain this is written for:

| Stage | Tool |
|---|---|
| Stills | ChatGPT image generation |
| Motion | Kling, Grok, Gemini (image-to-video from the stills) |
| Track | Suno |

Reference frames that came out of this pack: `reference/goblin-mandala.jpg`, `reference/nautilus-specimen.jpg`.

## Style lock

Paste in front of any still prompt:

> luminous techno-mysticism, sacred geometry fused with circuitry, liquid glass and chrome, radial explosion on pure black, fluorescence-microscopy palette of cyan magenta acid green and hot pink, heavy chromatic aberration and pixel-sort, crystalline focal point, scientific imaging mixed with psychedelic render, optimistic not horror, midjourney-like detail

Avoid line. ChatGPT has no negative-prompt field, so append it as a sentence:

> Avoid grimdark, blood splatter, muddy browns, flat cartoon, soft studio lighting, watermark, and text.

(Drop "text" from the avoid line when you want the specimen-sheet readout look from the nautilus frame. Instead ask for "monospace lab-readout annotations in acid green at the corners".)

## Stills

**Goblin**
> Crystalline goblin face as a mandala center, glass tusks and circuit-veined ears, freckled pale skin with projected RGB traces, one exploding glass eye, radial shards of chrome teeth on black, fluorescence palette, pixel-sort at the edges.

**Zombie**
> Iridescent circuit-flesh zombie bust, skin like cracked liquid glass over glowing mycelium, MRI-grid halo, hexagonal cell grid of mutating faces behind the head, cyan and magenta false color, hard chromatic split, luminous not rotten.

**Vampire**
> Classical marble bust with a mechanical glass arm reaching into a data-storm, fang line as a thin neon circuit, rose-window collar of liquid chrome, black void, hot pink and electric blue only, scanline glitch across the eyes.

**Sea creature**
> Nautilus cross-section that is also a deep-sea creature, glass city inside the chambers, bioluminescent tendrils as circuit traces, radial eye at the spiral center, acid green and cyan on black, pixel-sorted water.

**Rider / eschaton**
> Silhouette on a horse riding toward a pixel-sorted rainbow creature made of data, dust in magenta, blue sky cracked with glitch, the creature's eye a crystalline mandala, hard color split, cinematic wide.

### Grid companions

For each hero still, generate one grid still with the same prompt plus:

> rendered as a 4-by-4 grid of the same creature, each cell a mutation of the last, identical framing, identical black background, no borders between cells

That gives you the snap target for the cut.

## Motion (image-to-video)

Feed the still, keep the motion prompt short, ask for 5 to 10 seconds. The camera moves, the glitch breathes, the subject barely does. Same prompt shape works in Kling, Grok, and Gemini. Kling takes a negative field: use the avoid line there.

**Goblin**
> Slow radial zoom into the central glass eye. Chrome shards rotate a few degrees around the face. Chromatic aberration pulses. Pixel-sort flickers at the frame edges. Face stays still, eye brightens.

**Zombie**
> Camera pushes in on the bust. Hexagonal faces in the background grid mutate one cell at a time. Mycelium glow pulses under the glass skin. MRI halo rotates slowly. No head movement.

**Vampire**
> Glass arm extends further into the data-storm. Scanline glitch sweeps across the eyes twice. Rose-window collar rotates. Hot pink and electric blue flicker. Bust stays still.

**Sea creature**
> Slow orbit around the nautilus. Tendrils drift as if underwater, trailing pixel-sort. Glass city lights flicker inside the chambers. Central eye mandala rotates. Lab readout text flickers.

**Rider / eschaton**
> Rider gallops forward in slow motion, dust rising in magenta. Rainbow data-creature grows and its eye mandala opens. Sky glitch cracks widen. Camera tracks with the rider, wide.

**Grid stills**
> Static camera. Each cell mutates in sequence, left to right, top to bottom. Hard color split on every change. No camera movement.

## Track (Suno)

Style field:

> uplifting glitch techno, 128 bpm, hard four-on-the-floor kick, sidechained synth pads, bitcrushed arpeggios, choir stabs, euphoric breakdown, datamosh risers, no vocals

Structure prompt or lyric field (instrumental markers):

> [Intro: filtered pads, 4 bars] [Drop: full kick, 16 bars] [Grid section: hi-hat rolls, 8 bars] [Breakdown: choir, 8 bars] [Drop: full kick, 16 bars] [Outro: pads decay]

The hard kick is your cut grid. The hi-hat rolls section is where the 4-by-4 grids go. The breakdown holds the software-chrome frame.

## Cut

Hard cuts on the beat. Snap between a single radial and a 4-by-4 grid of the same creature mutating. Radial zoom into the eye on the drop. Then a software-chrome frame (DAW timeline or old OS window) holding the sacred image for one bar.

Beat map for a 128 bpm track, one bar is 1.875 seconds:

| Section | Frame | Hold |
|---|---|---|
| Intro | hero still, slow zoom | 4 bars |
| Drop | hero clip, hard cut every beat between the five creatures | 16 bars |
| Grid section | 4-by-4 grids, cell mutations on hi-hats | 8 bars |
| Breakdown | software-chrome frame holding one hero still | 1 bar, then hero zoom into eye |
| Drop | repeat, reverse creature order | 16 bars |
| Outro | rider / eschaton wide, let the glitch fade | 4 bars |
