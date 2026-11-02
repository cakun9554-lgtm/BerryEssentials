# BerryEssentials 1.1.0

Paper plugin source. Build with `mvn clean package` (Java 21).

## Implemented in this build
- Live sidebar with configurable MiniMessage title/lines and the requested PROFILES / SERVER fields.
- Persistent wallet and bank balances, `/money`, `/bank deposit|withdraw`, `/pay`.
- Persistent clan creation/join/leave and clan name display.
- Configurable ranks, `/setrank`, scoreboard rank field, and Bukkit nametag team prefix/color sync.
- Persistent kills/deaths statistics for K/D.

## Commands
- `/money`
- `/pay <player> <amount>`
- `/bank`, `/bank deposit <amount>`, `/bank withdraw <amount>`
- `/clan create <name>`, `/clan join <name>`, `/clan leave`, `/clan info`
- `/setrank <player> <rank>` (permission `berryessentials.rank`)
- `/sethome`, `/home`, `/delhome`, `/setwarp`, `/warp` are declared for future expansion only in this build.

## Notes
- Paper API dependency is pinned to 1.21.4; test against a staging server matching that API before production.
- Rank sync here uses Bukkit scoreboard teams. It is not a LuckPerms group bridge or a TAB integration.
- K/D displays kills divided by deaths; when deaths are zero, it displays kills as `kills/0`.
- No land-claim feature is included.
