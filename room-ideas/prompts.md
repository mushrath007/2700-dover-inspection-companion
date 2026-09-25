# New room concepts: prompt and review guide

The complete copy-ready prompt for every room is stored in `manifest.json` and is also available from the **Copy image prompt** button on `new-room-ideas.html`. This guide defines the shared intent and the review gate that applies to every output.

## Design intent

- Furnish only the three upper bedrooms; use the lower photographed bedroom as an office.
- Plan two shared children's rooms with two genuine nightly sleeping surfaces in each room.
- Keep every room minimal, affordable, washable, easy to reset and free of unnecessary screens.
- Express Islamic influence through restrained geometry, arches, proportion, hospitality and calm—not AI-generated Arabic, Qur'anic verses, sacred text or imitation calligraphy.
- Connect children with nature through a few carefully selected plants and one properly maintained aquarium, not several bowls or tiny tanks.
- Reuse seller furniture only when it passes the condition, odor, safety, completeness and price checks in the Furniture page.

## Source and output map

| Room | Edit target | Accepted output |
| --- | --- | --- |
| Family room | `listing-photos/photo-10.jpg` | `room-ideas/generated/family-room-concept.webp` |
| Quiet living and prayer room | `listing-photos/photo-12.jpg` | `room-ideas/generated/quiet-living-prayer-concept.webp` |
| Dining room | `listing-photos/photo-15.jpg` | `room-ideas/generated/dining-room-concept.webp` |
| Breakfast and homework nook | `listing-photos/photo-04.jpg` | `room-ideas/generated/breakfast-nook-concept.webp` |
| Primary bedroom | `listing-photos/photo-20.jpg` | `room-ideas/generated/primary-bedroom-concept.webp` |
| Shared children's room A | `listing-photos/photo-23.jpg` | `room-ideas/generated/shared-kids-room-a-concept.webp` |
| Shared children's room B | `listing-photos/photo-25.jpg` | `room-ideas/generated/shared-kids-room-b-concept.webp` |
| Lower office | `listing-photos/photo-27.jpg` | `room-ideas/generated/lower-office-concept.webp` |
| Screened porch | `listing-photos/photo-29.jpg` | `room-ideas/generated/screened-porch-concept.webp` |

PNG fallback names are listed in `manifest.json`. Do not rename or overwrite the source listing photos.

## Generation method

These are interior **edits**, not free-form generations. For each room:

1. Load only the matching source photo as Image 1.
2. Label Image 1 as the edit target.
3. Use the complete room prompt from `manifest.json` or the web page.
4. Generate one room at a time so the model receives one clear layout problem.
5. Reject a result that changes fixed architecture, conceals a suspected issue or invents an extra door/window.
6. If correction is needed, request one change and restate all critical invariants.

## Shared preservation constraints

- Remove existing movable furniture, decor and personal belongings.
- Preserve the camera angle, room proportions, walls, windows, doors, openings, flooring, ceiling, fixed trim and natural-light direction.
- Preserve visible areas that require inspection. A concept must not paint over, hide or falsely “repair” a ceiling, moisture or porch-roof concern.
- Keep walkways, stairs, doors, windows and emergency-exit paths clear.
- Use realistic furniture dimensions and a limited number of pieces.

## Privacy and content constraints

- No people, faces, names, addresses, family photos or readable personal documents.
- No logos, trademarks or watermarks in generated outputs.
- No Arabic, Qur'anic verses, sacred text or imitation calligraphy. Image models can produce incorrect or disrespectful text.
- Do not upload private inspection evidence or browser backup files. Only the public listing-room source named in the manifest is required.
- Strip image metadata before publishing an output.

## Child and nature safety

- No bunk or loft bed beneath a ceiling fan.
- Each shared children's room must visibly contain two proper nightly sleeping surfaces.
- Anchor dressers, bookshelves and other tip-over furniture to suitable wall structure.
- Prefer rounded edges, washable materials, cord control and unobstructed exits.
- Use only one lidded 10–20 gallon aquarium on a purpose-built, level stand. Cycle the tank before fish, use adult-led maintenance, provide GFCI protection and a drip loop, and avoid direct sunlight.
- Do not place an aquarium on a dresser, cube shelf or improvised table. Do not use a fish bowl.
- Possible lower-risk plant starting points include parlor palm, spider plant, calathea and peperomia, but verify the exact species against current child and pet guidance before purchase.

## Room-specific must-haves

### Family room

- Compact washable seating and movable floor cushions.
- Low closed book/toy storage and central floor play space.
- The home's single aquarium, correctly supported and away from direct sun.
- No television as the visual focal point.

### Quiet living and prayer room

- Flexible seating, low books and a closed bench for roll-away prayer mats.
- A generous open floor area.
- No invented qibla direction; verify orientation on site.

### Dining room

- Six wipe-clean seats, one realistically scaled table and one anchored closed cabinet.
- Clear chair pull-out space and unobstructed access to the sliding door.

### Breakfast and homework nook

- One compact table, a storage bench and two movable chairs.
- Hidden school/craft storage and both large openings kept clear.

### Primary bedroom

- Bed, two compact nightstands and at most one low dresser.
- Baseboard heat, HVAC, windows and door kept clear.
- Ceiling concern remains visible for inspection rather than cosmetically erased.

### Shared children's room A

- Two low twin beds, or one twin and a clearly shown nightly-rated trundle.
- Shared anchored dresser and compact two-place work surface.
- No bunk/loft bed and no obstruction at windows or exit.

### Shared children's room B

- Two separate low twin storage beds.
- One shared desk, one anchored low chest and one narrow book ledge.
- No television, gaming chair, bunk/loft bed or tall unanchored storage.

### Lower office

- Bed removed; one desk, ergonomic chair, low file cabinet and narrow anchored bookshelf.
- Ceiling concern must remain visible; furnishing waits until moisture verification is complete.
- Cables controlled and baseboard heat kept clear.

### Screened porch

- One weather-resistant table, six stackable chairs and one storage bench.
- No aquarium or indoor-only upholstery.
- Roof boards, skylight and other concern areas remain visible; repairs come before furnishing.

## Acceptance checklist for every generated image

- [ ] The room is clearly the same photographed room.
- [ ] Camera angle, walls, ceiling, windows, doors, flooring and fixed openings are unchanged.
- [ ] No inspection concern has been hidden or falsely repaired.
- [ ] Doors, windows, stairs and walking paths remain clear.
- [ ] Furniture is realistically scaled and the room is not crowded.
- [ ] Child-room image shows two safe sleeping surfaces and no bed under fan blades.
- [ ] Tall storage appears anchorable and cords do not create hazards.
- [ ] Aquarium, if present, is the single properly supported lidded tank described above.
- [ ] No people, faces, names, address, personal photos or readable documents appear.
- [ ] No generated Arabic, sacred text, logo, trademark or watermark appears.
- [ ] File metadata has been stripped and the file uses the exact manifest filename.
