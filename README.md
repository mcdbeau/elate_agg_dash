# Elate Store Dashboards

A single static page (`index.html`) that shows six store service dashboards from elatemcd.com side by side.

- **Phone:** the tiles stack and you scroll through them in order.
- **900px and wider:** 2 columns × 3 rows, fitting the screen.
- **1400px and wider:** 3 columns × 2 rows, fitting the screen.
- Each tile has a store-number header and an "Open ↗" link to that dashboard.
- The page reloads every dashboard every 5 minutes (set `AUTO_REFRESH_MINUTES` in `index.html`), and the "Refresh all" button reloads them on demand.

## Passwords

No passwords are stored in this repo. They go in the part of the link after `#`, which the browser never sends to the server:

```
https://mcdbeau.github.io/elate_agg_dash/#4453=PASSWORD&4578=PASSWORD&10514=PASSWORD&11785=PASSWORD&11960=PASSWORD&18056=PASSWORD
```

A store with no password in the link shows a "No password" message. Keep the full link private and bookmark it on each device.

## Editing stores

Edit the `STORES` list near the bottom of `index.html`, and add or remove the matching `store=password` pair in your link.

## Deploying

The site is published by GitHub Pages from the `main` branch, root folder (**Settings → Pages**).
