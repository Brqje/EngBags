# EngBags
EngBags - 2019 Baroque edit

One-bag with item type auto-sort. I've modded it to use sensible categorization/auto sorting for both leveling and end-game TBC 2.4.3. It's modified for all the requirements of a serious TBC end-game raider, presenting inventory contents in a streamlined way.

Modifications:

- Modified OpenAllBags hook to allow Blizzard "Open All Bags" keybind to actually toggle, instead of just open bags (similar to default UI behaviour)
- Modified default settings: columns from 9 to 10
- Modified default color settings: background and borders from blue to dark gray
- Modified categorization groups
- Modified categorization string search patterns
- Added nearly 400 items to specifically categorize (default override)

The general idea is that similar consumables should be grouped. The same applies to tokens and class items. Also, buffs which are generally clicked pre-combat (food buffs, elixirs, weapon buffs), are placed to the left, for easy ergonomic access. Potions and runes should always be keybound to action bars, so they're placed to the right. Item sorting is split between 15 groups, with most having subgroups as well:

15: explosives / 14: quiver & ammo bag projectiles, soul shards / 13: gray items, empty bag slots

12: boe items, class books, recipes, general reagents, tradegoods / 11: tradeskill, tradeskill created / 10: other soulbound

9: rogue poisons, weapon buffs / 8: other keys, quest items, misc items, tokens / 7: gear which has been equipped

6: flasks, battle elixirs, guardian elixirs / 5: bandages, other consumables / 4: potions, runes

3: food (including food buffs), drinks / 2: class reagents, projectiles / 1: hearthstone, passive class items, trade tools, mounts, mini pets

Within a group, subgroups are alphabetically sorted.
Within a subgroup, items are also alphabetically sorted.

**Shaman bag screenshot**

![img](https://imgur.com/zQmKP6A.jpg)

**Rogue bag screenshot**

![img](https://imgur.com/JzpVMVG.jpg)


**FAQ**

**Q:** I have a non-English WoW client. Why don't I get similar categorization results as in your screenshots/video?
**A:** EngBags' categorization relies heavily on string search patterns, thus being localization dependent. It's the foundation of how the addon works. I could add localization handling for other languages, but I'd need input.

**Q:** I've updated to a newer version, but item list categorization updates have no impact?
**A:** After updating, delete your setting files: \WTF\Account\ACCOUNTNAME\SavedVariables\EngBags.lua and EngBags.lua.bak
