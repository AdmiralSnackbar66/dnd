
## Basic 5e Layout

## Full example

```statblock
image: [[Ancient Black Dragon.jpg]]
name: Ancient Black Dragon
size: Gargantuan
type: dragon
subtype:
alignment: chaotic evil
ac: 22
hp: 367
hit_dice: 21d20
speed: 40 ft., fly 80 ft., swim 40 ft.
stats: [27, 14, 25, 16, 15, 19]
saves:
  - dexterity: 9
  - constitution: 14
  - wisdom: 9
  - charisma: 11
skillsaves:
  - perception: 16
  - stealth: 9
senses: blindsight 60 ft., darkvision 120 ft., passive Perception 26
languages: Common, Draconic
damage_resistances: bludgeoning, piercing, and slashing from nonmagical attacks
damage_immunities: fire, poison
condition_immunities: charmed, frightened, grappled, paralyzed, petrified, poisoned, prone, restrained
cr: 21
traits:
  - name: Amphibious
    desc: The dragon can breathe air and water
  - name: Legendary Resistance (3/Day)
    desc: If the dragon fails a saving throw, it can choose to succeed instead.
actions:
  - name: Multiattack
    desc: "The dragon can use its Frightful Presence. It then makes three attacks: one with its bite and two with its claws."
  - name: Bite
    desc: "Melee Weapon Attack: +15 to hit, reach 15 ft., one target. Hit: 19 (2d10 + 8) piercing damage plus 9 (2d8) acid damage."
  - name: Claw
    desc: "Melee Weapon Attack: +15 to hit, reach 10 ft., one target. Hit: 15 (2d6 + 8) slashing damage."
  - name: Tail
    desc: "Melee Weapon Attack: +15 to hit, reach 20 ft ., one target. Hit: 17 (2d8 + 8) bludgeoning damage."
  - name: Frightful Presence
    desc: "Each creature of the dragon's choice that is within 120 feet of the dragon and aware of it must succeed on a DC 19 Wisdom saving throw or become frightened for 1 minute. A creature can repeat the saving throw at the end of each of its turns, ending the effect on itself on a success. If a creature's saving throw is successful or the effect ends for it, the creature is immune to the dragon's Frightful Presence for the next 24 hours."
  - name: Acid Breath (Recharge 5-6)
    desc: The dragon exhales acid in a 90-foot line that is 10 feet wide. Each creature in that line must make a DC 22 Dexterity saving throw, taking 67 (15d8) acid damage on a failed save, or half as much damage on a successful one.
reactions:
  - name: Amphibious
    desc: The dragon can breathe air and water.
  - name: Legendary Resistance (3/Day)
    desc: If the dragon fails a saving throw, it can choose to succeed instead.
legendary_actions:
  - name: Detect
    desc: The dragon makes a Wisdom (Perception) check.
  - name: Tail Attack
    desc: The dragon makes a tail attack.
  - name: Wing Attack (Costs 2 Actions),
    desc: The dragon beats its wings. Each creature within 15 ft. of the dragon must succeed on a DC 23 Dexterity saving throw or take 15 (2d6 + 8) bludgeoning damage and be knocked prone. The dragon can then fly up to half its flying speed.
spells:
  - The archmage is an 18th-level spellcaster. Its spellcasting ability is Intelligence (spell save DC 17, +9 to hit with spell attacks). The archmage can cast disguise self and invisibility at will and has the following wizard spells prepared
  - Cantrips (at will): fire bolt, light, mage hand, prestidigitation, shocking grasp
  - 1st level (4 slots): detect magic, identify, mage armor*, magic missile
  - 2nd level (3 slots): detect thoughts, mirror image, misty step
  - 3rd level (3 slots): counterspell, fly, lightning bolt
  - 4th level (3 slots): banishment, fire shield, stoneskin*
  - 5th level (3 slots): cone of cold, scrying, wall of force
  - 6th level (1 slot): globe of invulnerability
  - 7th level (1 slot): teleport
  - 8th level (1 slot): mind blank*
  - 9th level (1 slot): time stop
  - "* The archmage casts these spells on itself before combat."
```

### Blank template

Copy the following, or insert the [[stats-5e]] template.

```statblock
name: 
size: 
type: 
subtype: 
alignment: 
ac: 
hp: 
hit_dice: 
speed: 
stats: []
saves:
  - 
skillsaves:
  - 
damage_vulnerabilities: 
damage_resistances: 
damage_immunities: 
condition_immunities: 
senses: 
languages: 
cr: 
traits:
  - []
spells:
  - description
  - spell level: spell-list
actions:
  - []
legendary_actions:
  - []
reactions:
  - []
```

## Basic Fate Core Layout

### Full Example

```statblock
layout: Basic Fate Core Layout
image: "[[bear.png]]"
name: Barathar
description: an awkward sunbear
aspects: "
  - Smuggler Queen of the Sindral Reach\n
  - A Mostly Loyal Crew\n
  - Remorse is For the Weak\n
  - [[My Ship, The Death Dealer]]\n
  - I've Got the Law in My Pocket"
temporaryAspects: "
  - Owes [[the PCs]] a favor\n
  - Current owner of [[the MacGuffin]]"
stress: [4, 5]
consequences:
  - name: Mild (2)
    desc: "Formerly fractured bone is still healing"
  - name: Moderate (4)
    desc: ""
  - name: Severe (6)
    desc: ""
skills:
  - name: Fantastic (+6)
    desc: "Deceive, Fight"
  - name: Superb (+5)
    desc: "Shoot, Burglary"
  - name: Great (+4)
    desc: "Resources, Will"
  - name: Good (+3)
    desc: "Contacts, Notice"
  - name: Fair (+2)
    desc: "Crafts, Stealth"
  - name: Average (+1)
    desc: "Lore, Physique"
stunts:
  - name: Takes One to Know One (Deceive)
    desc: "Use Deceive instead of Empathy to create an advantage in social situations."
  - name: Feint Master (Deceive)
    desc: "+2 to use Deceive to create an advantage in a physical conflict."
  - name: Riposte (Fight)
    desc: "If you succeed with style on a Fight defense, you can choose to inflict a 2-shift hit rather than take a boost."
items:
  - name: sword +1
    desc: ""
  - name: leather armor +1
    desc: "a scuffed [[leather armor]] with red linen undershirt"
```

### Blank template

## Generic OSR Layout

### Full Example

```statblock
layout: Generic OSR Layout
name: The Dreaded Goose
art: image.png
hd: 12
hp: 72
ac: 12
morale: 10
traits:
  - [Wants, to be left in peace!]
  - [Personality, Easily angered and murderous.]
actions:
  - [Honk, +9 to hit, 9 (3d6) damage to everyone who hears The Dreaded Goose.]
```

### Blank template

Copy the following, or use [[stats-osr]].

```statblock
layout: Generic OSR Layout
name: 
art: 
hd: 
hp: 
ac: 
morale: 
traits:
  - []
actions:
  - []
```

## Knave 2e Layout

This custom layout is for characters in the Knave 2e system.

### Full Example

```statblock
layout: Knave 2e
name: Cheddar
hp: 15
armor: 11
level: 3 
xp: 4000
str: 1
dex: 2
con: 2
int: 2
wis: 1
cha: 1
careers: Boatman and Antiquarian
traits:
  - [Garb, Stained]
  - [Mark, Acid Scar]
  - [Hair, Braided]
  - [Personality, Courteous, braggart, stubborn]
actions:
  - [item 1, 10' pole]
  - [item 2, instrument]
  - [item 3, paddle]
  - [item 4, ancient coin]
  - [item 5, antique flag]
  - [item 6, lore book]
  - [item 7, SPELL: Ukanmar's Marvelous Animating Frog Prison]
  - [item 8, SPELL: Zarphon's Sacred Darkening Cone]
  - [item 9, ]
  - [item 10, ]
  - [item 11, ]
  - [item 12, ]
```



Copy the following, or use [[stats-knave]].

```statblock
layout: Knave 2e
name: Name
hp: 1
armor: 10
level: 1
xp: 0
str: 0
dex: 0
con: 0
int: 0
wis: 0
cha: 0
careers: Grave robber
traits:
  - ["Build, Gaunt"]
actions:
  - ["Test, test item"]
```

## Cypher (Numenera PC) Layout

### Full Example

```statblock
layout: Numenera PC
name: Venus
image: [[numa-venus-token.png]]
descriptor: Mechanical
type: Nano
focus: Who Works miracles
armor: 2
tier: 1
effort: 1
xp: 0 
might: 7
mightedge: 0
speed: 11
speededge: 0
speedcost: 1
intellect: 18
intellectedge: 1
abilities:
- [Sense magic, You can sense whether the numenera is active in situations where its presence is not obvious. You must study an object or location closely for a minute to get a feel for whether the touch of the ancients is at work.]
- [Hedge magic, 1 Intellect point. You can perform small tricks: temporarily change the color or basic appearance of a small object, cause small objects to float through the air, clean a small area, mend a broken object, prepare (but not create) food, and so on. Action.]
- [Healing Touch, 1 Intellect point. With a touch, you restore 1d6 points to one stat Pool of any creature. This ability is a difficulty 2 Intellect task. Each time you attempt to heal the same creature, the task difficulty increases by one step. The difficulty returns to 2 after that creature rests for ten hours. Action.]
- [Ward, You have a shield of energy around you at all times that helps deflect attacks. You gain +1 to Armor. Enabler.]
cyphers:
- ["[[Gravity-nullifying spray]]", "Make a nonliving object float 1d20 feet in the air permanently."]
- ["[[Telepathy implant]]", "Communicate telepathically with one creature."]
- ["[[Teleporter (bounder)]]", "Teleport to a location you can see."]
skills:
- [Trained in understanding numa-numa (Nano), You are trained in understanding numanera.]
- [Inability (Mechanical), You have a manner or an aura that others find a bit unnerving. Any task involving charm, persuasion, or deception is hindered.]
equipment:
- [Clothing]
- [Armor, hides and furs]
- [Book, book about numa-numa]
- [Weapon, razor ring]
attacks:
- [Onslaught, 2 Intellect points. Attack a foe you see (physical/mental). If the attack is physical, you emit a short-range ray of force that inflicts 4 points of damage. If the attack is mental, you focus your mental energy to blast the thought processes of another creature within short range for 2 points of Intellect damage (ignores Armor). Action.]
- [Razor leaves, 2 physical damage (razor ring).]
```


### Blank template

Copy the following, or use [[stats-numenera-pc]].

```statblock
layout: Numenera PC
name: 
image: 
descriptor: 
type: 
focus: 
armor: 0
tier: 1
effort: 1
xp: 0 
might: 0
mightedge: 0
speed: 0
speededge: 0
speedcost: 0
intellect: 0
intellectedge: 0
abilities:
- [Ability, Description.]
cyphers:
- ["[[Cypher page]]", "Description."]
skills:
- [Skill, Description.]
equipment:
- [Equipment, Description]
attacks:
- [Attack, Description]
```

