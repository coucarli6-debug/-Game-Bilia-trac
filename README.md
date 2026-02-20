# PoolChain 🎱

> **A P2P Billiard Game built on Trac Intercom** — play pool with moves broadcast over the Intercom peer-to-peer sidechain network.

![PoolChain Screenshot](./screenshot.png)

---

## What is PoolChain?

PoolChain is an 8-ball billiard game where every shot is broadcast as a signed event over the **Trac Intercom P2P sidechannel**. Game state (ball positions, turn, score) is relayed to all connected peers and can be replicated via the durable state layer — making it a fully decentralized multiplayer pool game.

**Built on:** [Trac Intercom](https://github.com/Trac-Systems/intercom)

---

## Features

- 🎱 Full 8-ball billiard physics (collision, friction, pocket detection)
- ⚡ Real-time P2P move broadcasting via Intercom sidechannels
- 🔗 Game state synced to Intercom's replicated-state layer
- 🏆 Turn-based 2-player system with scoreboard
- 📡 Live Intercom network feed (peers, blocks, state deltas)
- 🎨 Dark neon-billiard aesthetic with smooth canvas animations

---

## How It Works

1. Each player connects as an Intercom node
2. When a player shoots, the cue velocity + power is signed and broadcast over a sidechain
3. Other peers receive the move event and simulate the same physics deterministically
4. Final ball positions are committed to the replicated-state layer after each turn
5. The 8-ball winner is announced network-wide

---

## Play

Just open `index.html` in your browser — no build step needed.

```bash
git clone https://github.com/YOUR_USERNAME/intercom
cd intercom
open index.html
```

---

## Intercom Skill File

See [`SKILL.md`](./SKILL.md) for agent instructions on how to interact with the PoolChain P2P game state.

---

## App Screenshot / Proof

> Game running locally — physics, pocket detection, turn system, and Intercom feed all functional.



---

## Trac Address

```
trac14ww6yqcu9rnfxx05jh93qk43jwr5an54s85ek6g2z769qtve7j6snvaspt

```

> Payouts for the awesome-intercom bounty should be sent to the address above.

---

## About This Fork

This repo is a fork of [Trac-Systems/intercom](https://github.com/Trac-Systems/intercom) with PoolChain added as a demonstration app of what can be built on the Intercom P2P agent stack.

**Date Created:** 2025  
**Project Name:** PoolChain  
**Category:** P2P Game / Entertainment dApp
