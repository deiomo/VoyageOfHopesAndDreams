# ❤️ Voyage Of Hopes and Dreams

**A whimsical, Undertale/Deltarune-inspired RPG preset for [SillyTavern](https://github.com/SillyTavern/SillyTavern).**

Hiya! 👋

Welcome to **Voyage Of Hopes and Dreams (VOHD)**, a preset built on **u/Kahvana's Voyage** and modified to capture the goofy spirit of Toby Fox's games.

VOHD combines turn-based **FIGHT, ACT, ITEM, and MERCY** combat with Voyage's **A-Life** and **Nemesis** systems to make a living world where NPCs have lives of their own—and might challenge you to a fight because they don't like your shoes.

It's intended to be **plug-and-play** and uses approximately **8k tokens** for its preset instructions, depending on your setup.

> **Status: Playable WIP.** The core experience is ready to try, but some features still need polishing. Feedback is welcome!

## ✨ What's Inside?

- **Undertale/Deltarune-inspired combat:** FIGHT, ACT, ITEM, MERCY, and alternating PLAYER/DEFENSE phases.
- **Encounters that don't require villains:** Friends, strangers, and otherwise decent people might fight you for ridiculous reasons—or no apparent reason at all.
- **An evolving world:** A-Life gives NPCs activities, goals, relationships, and offscreen developments.
- **Consequences:** Nemesis lets characters remember what happened, change their attitudes, and develop rivalries.
- **LV (Level of Violence):** Your power grows with confirmed kills, while the world becomes increasingly distrustful, quiet, and dark.
- **Actions Lists:** Occasional CYOA-style suggestions, including options that are completely stupid.
- **Optional HTML/regex interfaces:** Battle screens, player status, NPC profiles, scene information, location discoveries, news, and world activity.

## 🚀 Getting Started

1. Open **SillyTavern** and import the VOHD preset `.json` using its preset import option.
2. Select VOHD as your active preset and start an adventure with your preferred character and scenario.
3. Optionally import the accompanying **Regex** scripts through **Extensions → Regex** to enable the RPG-style visual interfaces.
4. Choose your preferred encounter-frequency toggle. **Frequent** is the intended default.
5. Start playing!

**Note:** The preset controls the AI's behavior. The visual interface scripts are a separate display layer; importing the preset JSON alone may not enable the HTML panels. The exact setup depends on the files included with the release.

## ⚔️ Combat

Combat is a major part of VOHD, and an encounter doesn't automatically mean you've met a bad guy. A friendly NPC might challenge you for a laugh, a misunderstanding, or no reason whatsoever.

### Encounter Frequency

Choose **one** of these optional settings:

| Mode | What to expect |
| --- | --- |
| **Balanced** | A mix of combat, exploration, conversations, and peaceful moments. |
| **Frequent** *(default)* | Lots of battles, including silly and unexpected challenges. |
| **Extremely Frequent** | Near-constant opportunities to fight, including rapid-fire absurd encounters. |

### PLAYER Phase

On your turn, the combat menu offers four commands:

| Command | What it does |
| --- | --- |
| **FIGHT** | Attack an opponent to reduce their HP. |
| **ACT** | Interact with an opponent through words, gestures, tricks, jokes, and other creative actions. **CHECK** reveals clues about how to pacify them, but uses your turn. |
| **ITEM** | Use something from your inventory. |
| **MERCY** | **SPARE** an opponent once their individual MERCY meter reaches **100%**. Sparing takes a turn; reaching 100% alone doesn't end their participation. |

ACT options are **suggestions**, not a restricted command list. You're welcome to invent your own actions and see what happens.

### DEFENSE Phase

After your action, surviving enemies get their turn. The PLAYER menu is replaced by **DEFENSE MODE**, offering:

- **DODGE** — avoid the incoming attack.
- **BLOCK** — reduce or prevent damage.
- **ITEM** — use an appropriate item defensively.

You can describe *how* you defend. Success depends on plausibility, timing, the environment, and your character's abilities.

> **Vague:** “I dodge.”
>
> **Better:** “I duck beneath the horizontal sword swing.”
>
> **Creative:** “I dive behind the stone pillar to avoid the fireball.”
>
> **Not automatically effective:** “I do seventeen backflips and become invincible.”

After the enemy's attack is resolved, the GM gives some enemy flavor text and returns to the PLAYER phase.

### Winning and Rewards

Win by **defeating opponents** or **sparing them**. Each enemy has their own MERCY percentage, and you must spend an action to SPARE them at 100%.

Winning grants **currency and a chance at items**, whether you use FIGHT or MERCY. The currency's name depends on your setting; it doesn't have to be G.

## ❤️ LV — Level of Violence

LV isn't a traditional experience-point system. It increases when the PC causes **confirmed kills**, not when enemies are spared or nonlethally defeated.

**Every 3 kills increases LV by 1.** LV never decreases.

As LV rises, the PC becomes stronger, but the world gradually changes. Whimsical scenes become less common, NPCs grow more suspicious or afraid, and once-lively places may become deserted.

| LV | Atmosphere |
| --- | --- |
| **1** | Innocence — colorful, lively, and absurd. |
| **2–4** | Unease — subtle tension and growing distrust. |
| **5–8** | Tainted — darker narration and increasingly visible power. |
| **9–12** | Dread — fear spreads; familiar places grow quieter. |
| **13–19** | Desolation — a lonely, oppressive world. |
| **20+** | **The Hollow World** — eerie silence and profound consequences. |

High LV **does not force your character to act violently**. You can still show mercy or try to make amends, but what happened before doesn't simply vanish.

## 🌎 A Living World

### A-Life

Inspired by **S.T.A.L.K.E.R.**'s A-Life system, the world continues beyond your immediate scene. NPCs pursue goals, build relationships, travel, and participate in events that can unfold offscreen.

### Nemesis

Inspired by **Middle-earth: Shadow of Mordor / Shadow of War**, NPCs remember what you do. Their relationships, traits, rivalries, reputation, and positions in the world can change over time.

### Actions Lists

Sometimes the GM will offer a short list of possible actions, ranging from sensible to absolutely ridiculous.

**You're standing in a swimming pool. What will you do?**

1. Swim around.
2. Dive underwater.
3. Splash someone nearby.
4. Relax by the poolside.
5. **Drink all the water in the pool.**

You're free to ignore every option and do something else. These are prompts for creativity, not limits on what you can attempt.

## 🖥️ Optional Visual Interfaces

VOHD includes optional HTML/regex presentation for:

- PLAYER, DEFENSE, and combat result screens
- PC status, HP, LV, kills, currency, equipment, and inventory
- NPC character profiles
- Location discovery sheets
- Scene information
- News bulletins
- A-Life/world activity
- Game Over

The interfaces are primarily **display-only**. Expanding a menu shows information; it does not automatically send an action to the AI. Type your chosen action into the chat as usual.

## ⚠️ Known Limitations / Work in Progress

- **Combat currently targets 1-vs-many encounters.** Companions may not receive their own commands or turns consistently. A Deltarune-style controllable party system is planned for a future update.
- **The AI is the game engine.** Combat outcomes, inventory, MERCY percentages, HP, and other persistent details are interpreted and tracked by the model. Mistakes and inconsistencies can happen.
- **Visuals require setup.** The HTML/regex interfaces may need to be imported separately, and compatibility can depend on SillyTavern configuration.
- **This is still being polished.** Balance, turn consistency, and tracker behavior are all open to improvement.

If you run into bugs or have ideas, feel free to share feedback!

## 🙏 Credits

**Huge thanks to u/Kahvana** for creating the original **Voyage** preset. Without it, there would be no Voyage Of Hopes and Dreams. I also really enjoyed talking with them on Discord! 👋

VOHD takes creative inspiration from **Undertale** and **Deltarune** by Toby Fox, alongside **S.T.A.L.K.E.R.**'s A-Life and **Shadow of Mordor / Shadow of War**'s Nemesis systems.

This is an unofficial, fan-inspired preset and is not affiliated with or endorsed by those games' creators or publishers.

---

**I hope you enjoy the voyage!** ❤️
