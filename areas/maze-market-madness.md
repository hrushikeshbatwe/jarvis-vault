---
updated: 2026-08-31
---
# Maze Market Madness
- Wrote the GDD in 2024, scoped as a 3-4 month project; wants to build a prototype now to test if it works
- Concept: timed grocery run through a randomized haunted supermarket ("Haunt Heaven Hyper Mart"), player-selectable floor count up to 10, puzzles tied to each floor's items, money from partner as the purse, discounts for solved puzzles, limited skips per floor
- Planned 10 interactable NPC types that taunt, give coupons for quests, and turn hostile if disrespected
- Planned DLC: "Deadly Edition" (traps, aggressive NPCs) and "Calm Mode" (intended to ship with main game)
- Prototype plan in the doc: start button → house intro → driving cutscene to the mart → core structure, physics and mechanics
- New addition he wants: multiplayer
- Frames this as a long-planned project, not a throwaway one, explicitly wants to avoid the plan-and-quit pattern
- Starting the prototype with the shopping loop, building the cart/inventory system in UE5 Blueprints first
- Using Wingman (UE5 in-editor AI assistant) alongside this
- Prototype loop working end-to-end: Cart map, ShoppingList map, live on-screen readouts for both, IsListComplete validation (tested with P key + Print String), GenerateShoppingList (random items via a shrinking Pool array, no repeats) wired to BeginPlay
- Known open item: ShoppingList currently lives on the Character BP; deliberately deferred moving it to round/GameState level until respawn or multiplayer becomes real
- Known open item: cart readout Text widget has overlapping/unpositioned lines in the UI, cosmetic only
- Flash-sale timer in progress: items get flagged at round start (weighted random chance) with a countdown; trigger is round-start for the prototype, NPC-proximity trigger deliberately deferred as a separate later task
- Revised approach: wants Claude to build the Blueprint node logic directly (via MCP) going forward rather than hand-typing every node himself, he enjoys designing logic, levels, and aesthetics, but dislikes the hands-on work of building/implementing that logic; superseded his earlier hand-build-only rule
- Long-term vision for the game: "ultimate shopping simulator", multiplayer chill chaos with sales, out-of-stock events, weird NPCs, rare items, and mazes; wants both solo and multiplayer support, with high replayability with friends
