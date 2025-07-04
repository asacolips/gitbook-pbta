# One Shot World

{% hint style="danger" %}
### THIS DOCUMENTATION IS NO LONGER USED

Go to [https://github.com/asacolips-projects/pbta/wiki/#getting-started](https://github.com/asacolips-projects/pbta/wiki/#getting-started) for the most current version of the documentation.
{% endhint %}

[One Shot World](https://yochaigal.itch.io/oneshotworld) is written by Yochai Gal and uses the [Creative Commons 4.0](https://creativecommons.org/licenses/by/4.0/) license.

![](../.gitbook/assets/image.png)

```
# Configure Rolls
rollFormula = "2d6"

# Configure stat toggle label and formula modifier.
[statToggle]
  label = "Disability"
  modifier = "-1"
  
# Define roll result ranges.
[rollResults]
  [rollResults.failure]
    range = "6-"
    label = "Miss"
  [rollResults.partial]
    range = "7-9"
    label = "Partial Success"
  [rollResults.success]
    range = "10+"
    label = "Success!"

########################################
## CHARACTERS ##########################
########################################
# Define the character group.
[character]

  # Define stats.
  [character.stats]
    str = "STR"
    int = "INT"
    con = "CON"
    dex = "DEX"
    wis = "WIS"
    cha = "CHA"

  # Define attributes.
  [character.attributesTop]
    [character.attributesTop.hp]
      type = "Resource"
      label = "Hit Points"

    [character.attributesTop.armor]
      type = "Number"
      label = "Armor"
    [character.attributesTop.damage]
      type = "Roll"
      default = "d4"
    [character.attributesTop.xp]
      type = "Xp"
      label = "Xp"
      max = 4

  # Define sidebar details.
  [character.attributesLeft]
    [character.attributesLeft.look]
      type = "LongText"
      label = "Look"
      
    [character.attributesLeft.goal]
      type = "LongText"
      label = "Personal Goal"
      
          [character.attributesLeft.drive]
      type = "LongText"
      label = "Drives"
      
    [character.attributesLeft.memory]
      type = "LongText"
      label = "A Memory that made you"
      
    [character.attributesLeft.knowledge]
      type = "LongText"
      label = "Area Knowledge"

  # Define groups for moves.
  [character.moveTypes]
    basic = "Basic Moves"
    class = "Class Moves"
    advances = "Advances"

  # Define groups for equipment.
  [character.equipmentTypes]
    gear = "Starting Gear"
    optional = "Optional Gear"

########################################
## NPCS ################################
########################################
# Define stats.
[npc]
  # Define attributes.
  [npc.attributesTop]
    [npc.attributesTop.hp]
      type = "Resource"
      label = "HP"
    [npc.attributesTop.armor]
      type = "Number"
      label = "Armor"
    [npc.attributesTop.damage]
      type = "Roll"
      label = "Damage"
      default = "d6"
      
  [npc.attributesLeft]
    [npc.attributesLeft.traits]
      type = "LongText"
      label = "Traits"
    [npc.attributesLeft.instinct]
      type = "LongText"
      label = "Intinct"
      
    [npc.attributesLeft.knacks]
      type = "LongText"
      label = "Knacks"

  # Define logical groups for moves.
  [npc.moveTypes]
    gm = "GM Moves"
```
