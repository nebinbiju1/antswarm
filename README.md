# Ant Swarm

An interactive swarm-intelligence sandbox where 60 stigmergic ants lay and follow evaporating pheromone trails — drag to draw walls and watch emergent collective path-finding around obstacles.

**[Try it live →](https://nebinbiju1.github.io/antswarm/)**

## Controls
- **Drag** — draw walls
- **Right-drag** — erase walls
- Ants spawn on the left and travel east, finding their way around whatever you build.

## What's going on under the hood
- **Stigmergy** — ants communicate only by depositing pheromone in the environment.
- **Reaction–diffusion** — the pheromone field diffuses and evaporates each frame.
- **Sensor-based steering** — each ant samples three points ahead (left, center, right) and turns toward the strongest trail (Jeff Jones' Physarum-style sensing).
- **Wall-following** — when blocked, ants slide along obstacles in whichever direction is more goal-aligned.

See [index.html](index.html) for the full implementation — it's a single self-contained file.
