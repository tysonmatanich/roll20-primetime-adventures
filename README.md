# roll20-primetime-adventures

Customizable blueprint themed [Roll20](https://roll20.net/) character sheet and roll template for [Primetime Adventures](https://gshowitt.itch.io/primetime-adventures), the one-page RPG by Grant Howitt.

## Character Sheet

No need to keep track of numbers. Click the left and right "+" buttons to increase your primary or secondary stats (eg bear vs criminal).

When its time to roll dice, click one of the four buttons depending on if it uses your primary (bear) or secondary (criminal) stat. The "special" buttons roll 2d6 and keep the lowest (best) number.

| Default | Customized (squirrel themed) |
| --- | --- |
| <img width="400" alt="Character sheet example" src="assets/screenshots/character-sheet/primetime-adventures.png" /> | <img width="400" alt="Customized character sheet example" src="assets/screenshots/character-sheet/walnut-break.png" /> |

## Roll Template

Designed to be glanceable to easily determine success vs failure and which stat was used. For a "special" roll (advantage) 2d6 keep-lowest, you can hover over the red or green boxes to see the results of both dice.

### Default Roll Template

| Primary (Bear) | Secondary (Criminal) |
| --- | --- |
| <img width="250" alt="Bear roll template example" src="assets/screenshots/roll-template/bear.png" />                 | <img width="250" alt="Criminal roll template example" src="assets/screenshots/roll-template/criminal.png" />                 |
| <img width="250" alt="Bear special roll template example" src="assets/screenshots/roll-template/bear-special.png" /> | <img width="250" alt="Criminal special roll template example" src="assets/screenshots/roll-template/criminal-special.png" /> |

### Themed Roll Template

| Primary (Squirrel) | Secondary (Thief) |
| --- | --- |
| <img width="250" alt="Bear roll template example" src="assets/screenshots/roll-template/primary.png" />                 | <img width="250" alt="Criminal roll template example" src="assets/screenshots/roll-template/secondary.png" />                 |
| <img width="250" alt="Bear special roll template example" src="assets/screenshots/roll-template/primary-special.png" /> | <img width="250" alt="Criminal special roll template example" src="assets/screenshots/roll-template/secondary-special.png" /> |

## Roll20 Attributes

The templates were created to be customizable via attributes to use for other creature types. This can be set on a per sheet basis or game level via `useroptions` game settings. This can be useful for NPCs or for a heist not invloving bears.
### Attributes useful for customization:
`game_name`, `primary_type`, `secondary_type`, `label_1`, `label_2`, `label_3`, `label_4`, `label_5`, `label_notes`

### Other attributes:
`primary` (number 1-6), `secondary` (number 1-6), `character_name`, `text_1`, `text_2`, `text_3`, `text_4`, `text_5`, `text_notes`, `is_primary_bear` (auto set on sheet open)

## Macros for NPCs
See  [assets/macros.md](assets/macros.md) for more info.

## Known Issues
* Field `is_primary_bear` only updates on sheet open as Role20 doesn't trigger an update on field change.
* Accessible tooltip text could be better but Role20 doesn't (to my knowledge) provide a way of using field attributes in `alt` or `title` text

## Dungeon Scrawl Styles

Feel free to use [map-styles.ds](map-styles.ds) with [Dungeon Scrawl](https://probabletrain.itch.io/dungeon-scrawl) to create custom RPG maps that match the style used in this template.

## Development

To edit, update the files in `/html` and `/styles` then run `npm run build` which will generate new versions of [primetime-adventures.css](primetime-adventures.css) and [primetime-adventures.html](primetime-adventures.html).

## Credits

- Primetime Adventures was created by [Grant Howitt](https://twitter.com/gshowitt)

- Background texture created using [Dungeon Scrawl](https://probabletrain.itch.io/dungeon-scrawl) and then using [Repeater](https://www.richardwestenra.com/repeater/) to help turn it into a seamless repeating background image

- Bear icons ([bear-icon-7](https://www.mcicon.com/product/bear-icon-7/) and [bear-icon-28](https://www.mcicon.com/product/bear-icon-28/)) are customized artwork derived from [MCIcon](https://mcicon.com/)

- [Heart](https://www.flaticon.com/free-icon/cardiogram_3004451) and [gear](https://www.flaticon.com/free-icon/settings_503849) icons derived from [Freepik](https://www.freepik.com) from [flaticon.com](https://www.flaticon.com/)
