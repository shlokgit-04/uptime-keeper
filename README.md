# uptime-keeper

GitHub Actions keep-alive pinger for Shlok Vane's free-tier hosted projects.

Render's free web services spin down after 15 minutes without traffic and take
about a minute to spin back up. This repo runs a scheduled workflow that pings
the flagship service every 10 minutes so it never spins down.

Render's free plan allows about 750 instance-hours per workspace per month,
which is enough to keep exactly one service awake around the clock. Other
services are left to sleep (they wake automatically on the next request) until
they are migrated to hosts that do not sleep.

Made by [Shlok V.](https://shlok.is-a.dev)
