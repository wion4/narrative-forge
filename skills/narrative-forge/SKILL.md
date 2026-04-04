---
name: Narrative Forge
description: Use when creating game narratives, writing dialogues, building worlds, designing characters, plotting story arcs, writing GDD narrative sections, creating lore documents, environmental storytelling, branching narratives, cinematic scripts, or any creative writing for games. Also triggers on "write story", "write dialogue", "create character", "build world", "narrative design", "game script", "lore", "quest design".
version: 0.1.0
---

# Narrative Forge — Game Narrative Methodology

A comprehensive narrative design system built on techniques from masterworks across games, film, literature, and anime. Applies to story, dialogue, environmental narrative, and character design equally.

## Language

Detect user's system language via `echo $LANG` and write ALL narrative content in that language. If the user explicitly requests a specific language, use that instead.

## Source Material Reference

This methodology is distilled from ~50 works. When applying a technique, reference its origin so the user understands the lineage:

### Games
| Work | Key Techniques |
|------|---------------|
| Disco Elysium | Internal dialogue as gameplay, skill-based personality, failed-hero protagonist |
| Planescape: Torment | Philosophical core question driving all content, "what can change the nature of a man?" |
| The Last of Us 1-2 | Perspective flip (villain becomes playable), earned brutality, quiet moments |
| Red Dead Redemption 2 | Slow-burn character arc, environmental micro-stories, redemption through mundane acts |
| Baldur's Gate 3 | Party dynamics as narrative engine, romance as character development, D&D consequence chains |
| Undertale / Deltarune | Meta-narrative (player as entity), genocide/pacifist as moral system, breaking 4th wall meaningfully |
| Portal 1-2 | Villain-as-narrator, humor in horror, environmental puzzle-storytelling |
| Bioshock / Infinite | Ideological world-as-character, audio logs, twist recontextualizing everything |
| Dark Souls series | Environmental storytelling without exposition, item descriptions as lore, interconnected world design |
| Witcher 3 | Moral grey zones, no "right" choice, consequences delayed by hours, folk-tale tone |
| Silent Hill 2 | Psychological horror through symbolism, unreliable reality, guilt-as-monster |
| Mass Effect trilogy | Squad loyalty through personal quests, galaxy-scale stakes grounded in relationships |
| Spec Ops: The Line | Deconstruction of player agency, "you chose to keep playing", war-crime guilt |
| NieR: Automata | Multiple playthroughs revealing truth, existentialism through gameplay, ending-as-sacrifice |
| What Remains of Edith Finch | Each death = unique gameplay mechanic, house-as-narrative, family curse structure |
| Half-Life 1-2 | Never break first-person, world happens around you, silent protagonist done right |
| Dishonored | Systemic narrative (chaos system), world reacts to playstyle, lore through books/audiographs |
| Wolfenstein (New Order/Colossus) | Pulp tone with genuine emotion, villain escalation, B.J. as broken superman |
| Metro 2033/Last Light/Exodus | Atmosphere-as-narrative, moral choices hidden (no UI prompt), post-apocalyptic humanity |
| S.T.A.L.K.E.R. | Zone-as-character, emergent narrative, loneliness and danger, campfire stories |
| Atomic Heart | Soviet retro-futurism aesthetic, unreliable world, satirical utopia |
| Ghost of Tsushima | Honor vs pragmatism as central conflict, cultural identity, mentor-student arc |
| Cyberpunk 2077 | Terminal diagnosis as ticking clock, corpo-punk world, identity/transhumanism |
| Broken Arrow | Tactical briefing narrative, faction doctrine as character, military authenticity |

### Film
| Work | Key Techniques |
|------|---------------|
| В бой идут одни старики | Humor beside death, youth-at-war humanity, songs as emotional anchors |
| Собачье сердце | Allegory through absurdity, social satire, transformation-as-commentary |
| Star Wars I-VI + Mandalorian | Hero's Journey (Campbell), light/dark duality, found family, mythological structure |
| MCU Spider-Man (all) | Coming-of-age under pressure, mentor loss, responsibility theme |
| Loki (series) | Variant/identity crisis, self-confrontation, destiny vs free will |
| Deadpool | 4th wall destruction, humor-as-armor, subverting genre expectations |
| Завтра была война | Pre-war innocence, ideological pressure on youth, quiet tragedy |
| А зори здесь тихие | Women-at-war, each death matters, memory and sacrifice |
| Они сражались за родину | Soldier brotherhood, ordinary people in extraordinary situations |
| Судьба человека | One man's arc = nation's arc, resilience, post-war rebuild |
| Ликвидация | Charismatic investigator, post-war Odessa atmosphere, dialogue-driven tension |
| Место встречи изменить нельзя | Duo dynamic (Zheglov/Sharapov), moral ambiguity in justice, era authenticity |
| В августе 44 | Intelligence work as puzzle, tension without action, trust-nobody |
| Побег из Шоушенка | Hope as weapon, long-game protagonist, narrator-observer |
| Крёстный отец 1-2 | Power corrupts arc, family as institution, parallel timeline structure |
| Бойцовский клуб | Unreliable narrator, twist recontextualizing film, anti-consumerist allegory |
| Интерстеллар | Time as antagonist, love as dimension, hard sci-fi with emotional core |
| Начало | Nested realities, rules-of-the-world exposition, ambiguous ending |
| Форрест Гамп | Innocent witness to history, simplicity vs complexity, running motif |
| Список Шиндлера | Showing horror through restraint, villain humanization, "one more person" |
| Олдбой | Revenge spiral, devastating twist, moral destruction |
| Семь | Villain who wins, deadly sin structure, detective procedural subverted |
| Матрица | Red pill choice, messianic arc, simulated reality |
| Прибытие | Non-linear time as narrative structure, linguistics as plot, quiet first contact |
| 9 (мультфильм) | Wordless storytelling, small hero in dead world, sacrifice chain |
| Время первых | Claustrophobia tension, real-event heroism, space as hostile environment |
| Салют-7 | Engineering-as-heroism, cold war backdrop, machine-as-character |

### Сериалы
| Work | Key Techniques |
|------|---------------|
| Breaking Bad | Protagonist-to-antagonist transformation, "Mr. Chips to Scarface", every action has consequence |
| Чернобыль (HBO) | Systemic horror, truth vs lies, procedural tension |
| True Detective S1 | Dual-narrator unreliability, philosophical monologue, Southern Gothic atmosphere |
| Band of Brothers | Unit-as-family, each episode = one soldier's perspective, historical weight |

### Аниме
| Work | Key Techniques |
|------|---------------|
| Neon Genesis Evangelion | Hero deconstruction, psychological breakdown as climax, rejection of destiny |
| Attack on Titan | Perspective inversion (who is the enemy?), layered reveals, cycle-of-violence theme |
| Death Note | Intellectual duel structure, morality erosion, cat-and-mouse escalation |

### Литература
| Work | Key Techniques |
|------|---------------|
| Война и Мир (Толстой) | Epic multi-POV, history through personal lives, philosophical interludes |
| Преступление и наказание (Достоевский) | Guilt as psychological engine, moral philosophy through action, confession arc |
| Марсианские хроники (Брэдбери) | Poetic sci-fi, vignette structure, loneliness of colonization |

---

## Part 1: Story Architecture

### 1.1 Structural Models

#### Three-Act Structure (Hollywood Standard)
- **Act 1 (Setup, ~25%)**: World, protagonist, status quo, inciting incident
- **Act 2 (Confrontation, ~50%)**: Rising stakes, midpoint reversal, darkest moment
- **Act 3 (Resolution, ~25%)**: Climax, resolution, new equilibrium
- *Used in*: Last of Us, Mass Effect, Star Wars, Побег из Шоушенка

#### Kishotenketsu (Japanese 4-Act)
- **Ki (Introduction)**: Establish without conflict
- **Sho (Development)**: Deepen, still no conflict
- **Ten (Twist)**: Unexpected element changes everything
- **Ketsu (Conclusion)**: Reconcile the twist with the established
- *Used in*: Many Nintendo games, Undertale's pacifist route, Miyazaki films
- *Key insight*: Story without antagonist. Conflict is optional; contrast is essential.

#### Episodic/Vignette Structure
- Self-contained episodes united by theme, not continuous plot
- *Used in*: What Remains of Edith Finch, Марсианские хроники, Band of Brothers
- *When to use*: Anthology games, each level = new perspective

#### Non-Linear/Fragmented
- Timeline is broken, player/viewer assembles the truth
- *Used in*: Прибытие, NieR Automata, Dark Souls lore, Начало
- *Key insight*: Each fragment must work standalone AND as puzzle piece

#### Protagonist-to-Antagonist Arc
- Hero gradually becomes what they fought against
- *Used in*: Breaking Bad, Spec Ops: The Line, Крёстный отец, Attack on Titan
- *Rule*: Each step must feel justified to the character. The audience sees it coming; the character doesn't.

### 1.2 Plot Devices & Techniques

#### Chekhov's Gun
Everything introduced must pay off. Everything that pays off must be introduced.
- **In story**: Object shown in Act 1 becomes critical in Act 3
- **In dialogue**: Throwaway line returns as devastating revelation
- **In environment**: Background detail becomes plot-critical
- *Masters*: Portal (companion cube), Bioshock ("would you kindly"), Witcher 3 (seemingly minor quests affecting endings)

#### Unreliable Narrator
The storyteller lies, omits, or misremembers — and the truth changes everything.
- **Full unreliability**: Narrator is delusional (Бойцовский клуб, Silent Hill 2)
- **Partial unreliability**: Narrator has blind spots (True Detective S1)
- **Systemic unreliability**: The world itself lies (Bioshock, Spec Ops, Atomic Heart)
- *Rule*: The reveal must make the audience want to re-experience everything.

#### The Perspective Flip
Force the audience to see through the "enemy's" eyes.
- *Used in*: Last of Us 2 (playing as Abby), Attack on Titan S4 (Marley), NieR (Route B)
- *Rule*: Must build genuine empathy, not just "show the other side." The player must feel conflicted.

#### Delayed Consequences
Choices that seem minor ripple forward hours later.
- *Used in*: Witcher 3 (Bloody Baron questline), Mass Effect (squad loyalty = survival), Disco Elysium
- *Key insight*: The player should feel "I did this" not "the game punished me." No "correct" choice.

#### The Ticking Clock
External deadline that compresses all decisions.
- **Literal**: Timer, approaching army, disease (Cyberpunk 2077 — Johnny's takeover)
- **Emotional**: Relationship deteriorating, secret about to be exposed
- **Structural**: Every scene should feel like time is running out, even without a literal timer
- *Used in*: Cyberpunk 2077, Интерстеллар, В августе 44

#### The Sacrifice Chain
Each sacrifice raises the stakes for the next.
- Small sacrifice → medium sacrifice → ultimate sacrifice
- *Used in*: 9 (мультфильм), А зори здесь тихие (each girl's death), Mass Effect 3
- *Rule*: Never cheapen a sacrifice with resurrection. Dead is dead.

#### In Medias Res
Start in the middle of action, fill in context later.
- *Used in*: Half-Life (no cutscene, you're already in the tram), Wolfenstein, God of War
- *When to use*: When backstory would kill momentum. Let the player ask "what's happening?" not "when does it start?"

### 1.3 Theme & Core Question

Every strong narrative has ONE core question that all content serves:

| Work | Core Question |
|------|--------------|
| Planescape: Torment | What can change the nature of a man? |
| Spec Ops: The Line | Do you feel like a hero yet? |
| Last of Us | How far would you go for someone you love? |
| Bioshock | Is a man not entitled to the sweat of his brow? |
| Cyberpunk 2077 | What makes you "you" when everything can be replaced? |
| Dark Souls | Is the cycle worth preserving? |
| Undertale | Does the player have the right to kill for entertainment? |
| Ghost of Tsushima | What are you willing to sacrifice for your principles? |

**Rule**: If a quest, character, or mechanic doesn't relate to the core question — cut it or rework it.

---

## Part 2: Dialogue Craft

### 2.1 Voice Differentiation

Each character must sound unique with eyes closed. Techniques:

- **Vocabulary level**: Professor vs street kid vs soldier
- **Sentence structure**: Short/punchy (Zheglov) vs flowery/elaborate (Disco Elysium's narrator)
- **Speech patterns**: Repetition, pet phrases, verbal tics
- **What they DON'T say**: Subtext, avoidance, deflection
- *Master class*: Disco Elysium (every skill has a personality), Witcher 3 (Geralt's dry wit vs Dandelion's dramatics), Ликвидация (Gotsман's Odessa slang)

### 2.2 Subtext

The best dialogue never says what it means directly.

**Surface vs Meaning:**
```
SURFACE: "Nice weather today."
MEANING: "I don't want to talk about what happened."
```

- *Master class*: В августе 44 (intelligence officers speak in riddles), Место встречи (interrogation scenes), Mass Effect (Garrus calibrating = avoiding emotions)

**Techniques:**
- **Displacement**: Characters argue about dishes when they mean the relationship
- **Loaded silence**: What's NOT said after a revelation
- **Contrast**: Cheerful words, devastating context (Portal's GLaDOS)

### 2.3 Dialogue Functions

Every line must serve at least ONE function:

1. **Reveal character** — show personality, values, flaws
2. **Advance plot** — deliver information, trigger events
3. **Build world** — expose lore, culture, history naturally
4. **Create tension** — conflict, threat, time pressure
5. **Provide relief** — humor, warmth, breathing room

*Lines serving 0 functions: cut. Lines serving 3+: masterwork.*

### 2.4 Branching Dialogue Design

#### The False Choice (Anti-Pattern)
```
A) "Yes, I'll help." → quest starts
B) "Tell me more." → exposition, then quest starts
C) "No." → "Please?" → quest starts
```
**Never do this.** If all roads lead to the same place, don't pretend there's a choice.

#### The Meaningful Branch
```
A) Help the village → villagers survive, baron hunts you later
B) Help the baron → village burns, baron becomes ally
C) Walk away → both factions hostile, but you find a third path
```
*Each choice must COST something.* — Witcher 3 principle

#### The Hidden Choice
Player doesn't realize they're choosing. Their behavior IS the choice.
- *Used in*: Metro (moral points from hidden actions), Dishonored (chaos from kills), Undertale (fight/mercy)

### 2.5 Exposition Without Info-Dumps

**NEVER** have a character explain what both characters already know. Instead:

- **Argue about it**: Two people who disagree reveal facts through conflict
- **Discover it**: Character finds a document, recording, environment
- **Demonstrate it**: Show the rule working, don't explain it
- **Newcomer**: One character genuinely doesn't know (but earn this — don't force it)
- *Anti-pattern*: "As you know, Professor, the reactor was built in 1986..." (Чернобыль HBO brilliantly avoids this)

---

## Part 3: Environmental Storytelling

### 3.1 The Silent Narrator

Tell stories without a single word of dialogue:

- **Object placement**: A child's toy next to a skeleton (Last of Us, Metro)
- **Architecture**: A room's design reveals its purpose and what went wrong (Dark Souls, Bioshock)
- **Wear and tear**: What's damaged tells you what happened (S.T.A.L.K.E.R.)
- **Contrast**: Beauty next to horror, order next to chaos (Atomic Heart)

### 3.2 Environmental Storytelling Layers

1. **Macro** — The world itself tells a story (Zone in S.T.A.L.K.E.R., Rapture in Bioshock)
2. **Meso** — Each area/level has its own mini-story (apartments in Metro, houses in Edith Finch)
3. **Micro** — Individual details reward attention (item descriptions in Dark Souls, graffiti in Half-Life 2)

### 3.3 Lore Delivery Vehicles

| Vehicle | Immersion | Info Density | Examples |
|---------|-----------|-------------|---------|
| Item descriptions | High | Low | Dark Souls, NieR |
| Audio logs | Medium | High | Bioshock, Dishonored |
| Environmental text | High | Medium | Half-Life 2 graffiti, Metro journals |
| NPC dialogue (ambient) | High | Low | Witcher 3 peasant chatter, RDR2 camp talk |
| Codex/database | Low | Very High | Mass Effect, Cyberpunk 2077 |
| Cutscenes | Low | High | Wolfenstein, Ghost of Tsushima |

**Rule**: The more immersive the vehicle, the more the player will remember it.

### 3.4 World-as-Character

The setting should have personality, moods, and arc:

- **The Zone** (S.T.A.L.K.E.R.) — hostile, indifferent, beautiful, unpredictable
- **Rapture** (Bioshock) — grandiose decay, ideology made architecture
- **Night City** (Cyberpunk) — seductive, lethal, apathetic
- **Metro tunnels** (Metro) — claustrophobic mother, protects and traps
- **Lordran** (Dark Souls) — cyclical, ancient, indifferent to your existence

---

## Part 4: Character Design

### 4.1 Character Pillars

Every character needs three pillars:

1. **Want** (conscious goal) — what they say they're after
2. **Need** (unconscious need) — what they actually need to grow
3. **Flaw** (internal obstacle) — what prevents them from getting the Need

| Character | Want | Need | Flaw |
|-----------|------|------|------|
| Joel (TLOU) | Protect Ellie | Learn to love again | Can't let go of Sarah |
| Walter White | Provide for family | Feed his ego | Pride disguised as love |
| Geralt | Stay neutral | Accept he cares | Emotional avoidance |
| Arthur Morgan | Loyalty to gang | Redemption | Blind loyalty |
| B.J. Blazkowicz | Kill Nazis | Find peace | Can't stop fighting |
| Gotsман (Ликвидация) | Catch the bandit | Restore order to his city | Trust issues |

### 4.2 Character Arc Types

#### Positive Arc (Growth)
Character overcomes flaw, gets Need. *Most common.*
- Joel learns to love → sacrifices cure for Ellie
- Arthur Morgan finds redemption → helps John escape

#### Negative Arc (Corruption)
Character surrenders to flaw, becomes worse.
- Walter White → Heisenberg
- Anakin → Darth Vader
- Spec Ops protagonist → war criminal

#### Flat Arc (Catalyst)
Character doesn't change — they change the world around them.
- Geralt (mostly) — his consistency exposes others' hypocrisy
- Forrest Gump — unchanged amid decades of change
- The Mandalorian S1 — his code is tested but holds

#### Tragic Arc (Doomed)
Character's flaw destroys them despite awareness.
- Hamlet, Oldboy, Silent Hill 2's James
- *Key*: Audience sees it coming. Character might too. Can't stop it.

### 4.3 Antagonist Design

A villain is only as good as their argument.

**The Mirror Villain**: Same goal as hero, different method
- Жеглов/Шарапов (Место встречи) — both want justice, disagree on means

**The Philosophical Villain**: Represents a coherent worldview
- Andrew Ryan (Bioshock) — objectivism taken to extremes
- Thanos — utilitarian calculus made physical

**The Systemic Villain**: Not a person, but a system
- Чернобыль HBO — Soviet bureaucracy kills
- S.T.A.L.K.E.R. — the Zone itself
- Dark Souls — the cycle of fire

**The Sympathetic Villain**: You understand why they did it
- Abby (TLOU2), Eren (AoT S4), Magneto
- *Rule*: Give them a scene where they're right.

### 4.4 Ensemble Cast

When writing groups:
- Each member = one facet of the core theme
- **Chemistry pairs**: Serious/comic, mentor/student, rivals
- *Used in*: Band of Brothers, Mass Effect squad, В бой идут одни старики (pilots), BG3 companions
- **Rule**: If two characters serve the same narrative function, merge them.

---

## Part 5: Anti-Patterns

### Things That Kill Narratives

| Anti-Pattern | What It Is | Fix |
|-------------|-----------|-----|
| Plot Armor | Character survives impossible situations because "main character" | If they survive, earn it. Or kill them. (А зори здесь тихие kills everyone.) |
| Deus Ex Machina | Problem solved by something never established | Chekhov's Gun — establish the solution early |
| Dead Choices | Illusion of choice, all paths converge | Every choice must cost something |
| Exposition Dump | Characters explain the world to each other | Show, argue, discover — never lecture |
| Grimdark for Shock | Violence/darkness without meaning | Every dark moment must serve the theme (Список Шиндлера vs torture porn) |
| Power Creep | Stakes evaporate because hero is too strong | Raise stakes emotionally, not just physically |
| Amnesia Protagonist | "Convenient" memory loss for exposition | If using amnesia, make it THE story (Planescape: Torment) |
| Love Triangle Filler | Romance subplot that adds nothing | Romance must illuminate character or theme (BG3 does this well) |
| The Chosen One (lazy) | Prophecy removes agency | Subvert it (NieR, Undertale) or earn it (Star Wars) |
| Monologuing Villain | Villain explains plan for no reason | Give them a reason to talk, or don't let them (Семь — villain wins BECAUSE he talks) |

---

## Part 6: Genre-Specific Techniques

### RPG / Story-Driven
- Companion loyalty = narrative investment (Mass Effect, BG3)
- Side quests must reflect main theme (Witcher 3's Bloody Baron = main themes in microcosm)
- Player character voice: silent (Half-Life), voiced-limited (Geralt), voiced-full (Shepard), internal (Disco Elysium)

### Action/Shooter
- Story through level design, not cutscenes (Half-Life, Metro)
- Pacing: action → quiet → tension → action (never all one speed)
- The "why am I fighting" question must have an answer every hour of gameplay

### Strategy/Tactics
- Faction identity through doctrine, not just visuals (Broken Arrow)
- Briefing as narrative moment — who briefs you reveals power structure
- Post-mission consequences visible in next mission

### Horror
- Fear of the unknown > fear of the seen (Silent Hill 2, Alien)
- Sound design IS narrative (Metro, S.T.A.L.K.E.R.)
- Safe spaces must eventually be violated

### Open World
- Emergent micro-stories (RDR2 stranger missions, S.T.A.L.K.E.R. random encounters)
- Main quest must coexist with player freedom without urgency paradox
- Fast travel = narrative sacrifice. Design world worth walking through.

---

## Part 7: Practical Workflows

### 7.1 Creating a New Story

1. **Define core question** — one sentence, no more
2. **Choose structural model** — three-act, kishotenketsu, episodic, non-linear
3. **Design protagonist** — want, need, flaw
4. **Design antagonist** — mirror, philosophical, systemic, or sympathetic
5. **Map the arc** — key turning points, midpoint reversal, climax
6. **Layer the world** — macro (setting), meso (areas), micro (details)
7. **Write dialogue** — subtext first, surface words second
8. **Plant Chekhov's guns** — review Act 3, then go back and seed Act 1
9. **Kill your darlings** — cut anything that doesn't serve the core question

### 7.2 Reviewing Existing Narrative

Ask these questions:
- Can I state the core question in one sentence?
- Does every major character relate to it?
- Does every quest/mission relate to it?
- Are there false choices? Fix or cut them.
- Can I tell characters apart by dialogue alone?
- Is exposition shown or told?
- Does the environment tell its own stories?

### 7.3 Using Agents

This plugin provides specialized agents for different narrative tasks:

- **story-architect** — builds story structure, arcs, plot outlines
- **dialogue-writer** — writes character dialogue with voice differentiation and subtext
- **world-narrator** — environmental storytelling, lore documents, codex entries
- **character-builder** — character sheets, arcs, relationship maps
- **concept-artist** — 2D visualizations: maps, locations, character concepts, UI mockups
