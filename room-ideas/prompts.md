# Whole-home concept review guide

The complete room list, source photographs, accepted image paths, plans, budgets and reusable prompts live in `manifest.json`. The web page renders that file directly.

## Current space map

| Space | Source | Selected concept |
| --- | --- | --- |
| Front exterior | `listing-photos/photo-01.jpg` | `generated/exterior-warm-white-concept.png` |
| Family hall | `listing-photos/photo-10.jpg` | `generated/family-hall-tv-nature-concept.png` |
| Prayer hall | `listing-photos/photo-12.jpg` | `generated/prayer-hall-zoned-concept.png` |
| Kitchen storage | `listing-photos/photo-18.jpg` | `generated/kitchen-white-pantry-concept.png` |
| Dining room | `listing-photos/photo-15.jpg` | `generated/dining-room-concept.png` |
| Breakfast nook | `listing-photos/photo-04.jpg` | `generated/breakfast-nook-concept.png` |
| Large three-bed room | `listing-photos/photo-20.jpg` | `generated/large-three-bed-nature-concept.png` |
| Compact adult bedroom | `listing-photos/photo-23.jpg` | `generated/compact-adult-bedroom-concept.png` |
| Upstairs study | `listing-photos/photo-05.jpg` | `generated/upstairs-study-concept.png` |
| Ground-floor office | `listing-photos/photo-27.jpg` | `generated/ground-office-four-screen-concept.png` |
| Full bathroom | `listing-photos/photo-07.jpg` | `generated/full-bath-refresh-concept.png` |
| Half bathroom | `listing-photos/photo-26.jpg` | `generated/half-bath-refresh-concept.png` |
| Sunroom aviary | `listing-photos/photo-29.jpg` | `generated/screened-porch-flight-aviary-concept.png` |
| Rear deck | `listing-photos/photo-31.jpg` | `generated/deck-eco-family-concept.png` |
| Side and rear garden | `listing-photos/photo-34.jpg` | `generated/side-garden-concept.png` |

The `photoVision` array in `manifest.json` covers photos 1–39 individually and links repeated angles back to these coordinated plans.

## Review every concept

- Confirm the room remains recognizably the photographed room and no fixed architecture has been invented.
- Measure door swings, closet access, drawer pull-out, heater and HVAC clearance before purchasing.
- Anchor storage, aquarium stands and monitor arms to suitable structure.
- Use Islamic geometry and arches as visual influence; never use AI-generated Arabic or sacred writing.
- Use only the family hall aquarium. It needs a fitted lid, dedicated stand, GFCI protection, drip loop and adult maintenance.
- Verify every plant species for children, pets and birds before purchase.
- Treat the sunroom as seasonal until a qualified person confirms that its roof, enclosure, electrical system and heating/cooling can support birds year-round.
- Keep cockatiels separated from hens and newly acquired birds; retain an indoor quarantine and recovery enclosure.
- Confirm the garden against a survey, utility marks, drainage, sunlight and local rules.
- Confirm the exterior siding material, manufacturer restrictions and surface condition before painting. Avoid dark paint on vinyl unless the coating and siding manufacturer permit it.
- Remove the white kitchen refrigerator through an appliance recycling route; retain only the stainless refrigerator if its condition and energy use are acceptable.

## Generation method

Use each listed source photograph as an edit target. Preserve camera angle, proportions, walls, windows, doors, flooring, ceiling, trim and natural-light direction. Change movable furnishings and decor only. Reject images that block an exit, hide an inspection concern, add readable personal information, or show unsafe furniture and animal arrangements.

The page prefers WebP and falls back to PNG. Save any new accepted output under the exact path in `manifest.json`, strip metadata, preview `../new-room-ideas.html`, and review the Git diff before publishing.
