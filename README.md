# Project EVOLVE Server v0.4.1

Paper 1.21.1 / Java 21.

This is the first EVOLVE Client integration build.

- The server no longer spawns Skeleton / Wither Skeleton / Wither as surrogate Monster bodies.
- The real Player remains authoritative for movement, HP, attacks, feeding and evolution.
- The player's private scoreboard carries a lightweight client marker:
  - `evolve_monster_s1`
  - `evolve_monster_s2`
  - `evolve_monster_s3`
  - `evolve_hunter`
- EVOLVE Client reads that marker and changes renderer/perspective.
- `/evolve monster` starts Stage 1.
- `/evolve levelup` changes Stage 1 -> 2 -> 3.
- `/evolve wildlife 6` keeps the existing wildlife/feed test.

Install the server JAR in `plugins/`.
EVOLVE Client is installed separately in each player's Fabric client.
