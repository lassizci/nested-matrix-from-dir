# nested-matrix-from-dir
Github Actions setup to run workflows sequentially and parallel based on numeric prefix:

Consider the following directory structure:
```
topdir
├── 10-base
├── 20-fourth
├── 20-second
├── 20-third
└── 30-fifth
```

This creates a matrix job that runs the following sequentially:
1) 10-base
2) 20-second, 20-third, 20-fourth in parallel
3) 30-fifth
