# Pixium Roadmap

> A collaborative pixel art canvas on the Stellar blockchain.

This roadmap outlines the planned milestones for Pixium from initial setup to production launch. Each milestone will be broken down into scoped GitHub issues across the four repos.

---

## v0.1 — Foundation ✳️ *Current*

The goal of this milestone is a working development environment and a deployable skeleton for all four repos.

- [ ] Repository setup (`onchain`, `backend`, `frontend`, `indexer`)
- [ ] Docker Compose dev environment (backend, frontend, Postgres, Redis, local Stellar node)
- [ ] CI pipelines — lint, build, and test for each repo
- [ ] Contributing guide, issue templates, and PR template
- [ ] Soroban contract: canvas initialization (width, height, palette, round duration)
- [ ] Soroban contract: `place_pixel(x, y, color)` with cooldown enforcement
- [ ] Backend: `GET /canvas` and `GET /pixel/:x/:y` endpoints
- [ ] Indexer: `PixelPlaced` event listener → PostgreSQL + Redis
- [ ] Frontend: wallet connection (Freighter) + canvas render + pixel placement

**MVP definition of done:** a player can connect their wallet, see the live canvas, place a pixel on-chain, and watch it appear for everyone in real time.

---

## v0.2 — Quests & Rewards

- [ ] Quest system: daily/weekly challenges that reward extra pixels
- [ ] Quest configuration (JSON-based, host-controlled)
- [ ] Quest completion verification (on-chain and off-chain variants)
- [ ] Backend: quest endpoints
- [ ] Indexer: `QuestCompleted` event handling
- [ ] Frontend: quest panel UI

---

## v0.3 — Leaderboards & Factions

- [ ] Global leaderboard (pixels placed, all-time and per-round)
- [ ] Faction creation and joining (on-chain)
- [ ] Faction pixel allocations — members share a pool
- [ ] Faction leaderboard
- [ ] Backend: leaderboard and faction endpoints
- [ ] Indexer: `FactionCreated` event handling
- [ ] Frontend: leaderboard sidebar and faction UI

---

## v0.4 — NFT Minting

- [ ] Players select a canvas region to mint as an NFT
- [ ] NFT metadata stored on-chain (Soroban)
- [ ] Off-chain image generation from canvas state
- [ ] Frontend: NFT minting flow and gallery viewer

---

## v0.5 — Color Voting

- [ ] Daily vote to add a new color to the palette
- [ ] On-chain vote tallying (Soroban)
- [ ] Indexer: `VoteCast` event handling
- [ ] New colors activated at the start of each day
- [ ] Frontend: color voting UI

---

## v0.6 — Templates

- [ ] Community templates: target image overlaid on the canvas
- [ ] Template bounties: fund incentives for completing a template
- [ ] Template progress tracking
- [ ] Frontend: template overlay UI

---

## v1.0 — Production Launch

- [ ] Multi-round support (new canvas each round)
- [ ] Full admin dashboard
- [ ] Production infrastructure (Kubernetes, monitoring, alerting)
- [ ] Security audit of Soroban contracts
- [ ] Public mainnet deployment on Stellar

---

Issues for each milestone will be posted to the relevant repo as we approach that milestone. Watch the repos or join the community to get notified.
