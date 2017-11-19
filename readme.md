# Lerna + yarn + workspaces = infinite loop

just
```
lerna bootstrap
```
and observe cli freezing.

# Tracks

Remove `"postinstall": "lerna bootstrap"` from `scripts` entry in [`package.json`](package.json) and bootstraping works.
The workspaces configuration seems a bit complex, but the heisenbug disapears in very simple setups. 
