# ImperialERA

ImperialERA is structured as an Ostranauts local mod bundle. The installed `Mods/` folder must contain `loading_order.json` and the `ImperialERA/` mod folder as siblings:

```text
loading_order.json
ImperialERA/
  mod_info.json
  data/
  images/
```

For local testing, do not leave `ImperialERA.zip` unopened inside `Ostranauts_Data/Mods/`. Extract or copy the zip contents into `Mods/` so `loading_order.json` sits directly at `Mods/loading_order.json` and the mod data sits at `Mods/ImperialERA/`.

The `ImperialERA|edit` entry in `loading_order.json` is intentional for local development. Ostranauts uses the `|edit` marker to identify local mods for the mod-list/upload workflow while still resolving the mod folder as `ImperialERA/`.

When making a distributable zip, package only `loading_order.json` and the `ImperialERA/` folder from this repository root. If the zip starts with an extra wrapper folder above `loading_order.json`, or if the zip is placed in `Mods/` without being extracted, Ostranauts will not detect the local mod.
