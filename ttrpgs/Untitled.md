```statblock
name: Prismari Pledgemage
size: Medium
type: Humanoid
class: Sorcerer
ac: 12 (15 with [[mage-armor-xphb|Mage Armor]])
hp: 66 (12d8 + 12)
speed: 35ft
stats:
  - 10
  - 15
  - 13
  - 12
  - 14
  - 17
saves:
  - Dexterity: 4
  - Charisma: 5
skillsaves:
  - Acrobatics: 4
  - Athletics: 4
  - Performance: 7
senses:
  - passive Perception 12
languages: 
  - Common plus any two languages
cr: 4
traits:
  - name: Evasion
    desc: If the pledgemage is subjected to an effect that allows it to make a Dexterity saving throw to take only half damage, the pledgemage instead takes no damage if it succeeds on the saving throw and only half damage if it fails, provided it isn’t incapacitated.
actions:
  - name: Multiattack
    desc: The pledgemage makes two Elemental Strike attacks.
  - name: Elemental Strike
    desc: _Melee or Ranged Spell Attack:_ +5 to hit, reach 5 ft. or range 60 ft., one target. _Hit:_ 12 (3d6 + 2) fire or cold damage (the pledgemage’s choice).
  - name: Showstopper (1/Day)
    desc: The pledgemage shines with elemental magic, targeting one creature it can see within 60 feet of itself. The target must make a DC 13 Wisdom saving throw. On a failed save, the target takes 28 (8d6) fire or cold damage (the pledgemage’s choice) and is stunned until the start of the pledgemage’s next turn. On a successful save, the target takes half as much damage and isn’t stunned
spells:
  - The pledgemage casts one of the following spells, requiring no material components and using Charisma as the spellcasting ability (spell save DC 13)
  - At will: [[minor-illusion-xphb|Minor Illusion]]
  - 2/day each: [[gust-of-wind-xphb|Gust of Wind]], [[silent-image-xphb|Silent Image]]
  - 1/day each: [[mage-armor-xphb|Mage Armor]], [[water-walk-xphb|Water Walk]]
bonus_actions:
  - name: Surge of Artistry (Recharge 4-6)
    desc: The pledgemage moves up to its speed, surrounding itself with elemental magic as it moves. Until the end of its turn, the pledgemage can move through the space of other creatures. The first time the pledgemage enters a creature’s space on a turn, that creature must succeed on a DC 13 Dexterity saving throw or be knocked prone. If the pledgemage ends its turn in another creature’s space, the pledgemage takes 5 (1d10) force damage and is pushed into the nearest unoccupied space.



```