# Database schema:
#### Entities:
- D&D book (has set of spells, aka spell list - but spell list per class?)
- individual spells

simpler to manage/interface with by having one big spell list, with data on source book+classes per spell

## Spell
- spell key ID
- name
- level (cantrip-9 or 0-9)
- school (conjuration, evocation, etc)
- casting time (1 action, 1 minute, etc)
- bool concentration
- bool ritual
- range (touch, self, self (10 foot radius), 30 ft, etc)
	- area/targets?
- components (V, S, M (a pinch of sand), M (consumed), etc)
	- cost of consumed components in gp?
- duration (instant, 1 round, 1 hour, concentation, etc)
- description/effect (various subheadings, "at higher levels")
- type of save, or if it's a spell attack, etc
- source book
	- page # in source book?
- spell in class's spell list - boolean fields?
	- arcane trickster (rogue archetype)
	- bard
	- cleric
	- druid
	- eldritch knight (fighter archetype)
	- paladin
	- ranger
	- sorcerer
	- warlock
	- wizard

#### Misc spell notes, 5e
ritual spells:
- don't use up a spell slot
- take 10 minutes longer to cast than normal
- caster must have a feature to cast rituals

material components:
- component pouch or spellcasting focus can be used in place of material components
- if a material component is consumed, the caster must have it for each cast
- must have a hand free for components/focus, but it can be the same hand for performing somatic components