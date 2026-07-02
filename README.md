# ImperialERA

ImperialERA is structured as an Ostranauts local mod bundle. The archive root must contain `loading_order.json` and the `ImperialERA/` mod folder as siblings:

```text
loading_order.json
ImperialERA/
  mod_info.json
  data/
  images/
```

When making a distributable zip, zip the contents of this repository root, not the enclosing repository folder. If the zip starts with an extra `ImperialERA/` wrapper above `loading_order.json`, Ostranauts will not detect the load-order file.
