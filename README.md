# Multiverse Parser

This module parses scene descriptions across various formats into each other using USD as the translation medium

## Usage

```bash
multiverse_parser --help
```

```bash
usage: multiverse_parser [-h] --input INPUT --output OUTPUT [--physics | --no-physics] [--visual | --no-visual] [--collision | --no-collision]
                         [--keepusd | --no-keepusd] [--collisionrgba COLLISIONRGBA [COLLISIONRGBA ...]]

Multiverse parser

options:
  -h, --help            show this help message and exit
  --input INPUT         Import scene description as (URDF, MJCF, WORLD or USD)
  --output OUTPUT       Export scene description as (URDF, MJCF, WORLD or USD)
  --physics, --no-physics
                        Whether to include physics properties or not
  --visual, --no-visual
                        Whether to include visual meshes or not
  --collision, --no-collision
                        Whether to include collision meshes or not
  --keepusd, --no-keepusd
                        Whether to keep the USD file or not
  --collisionrgba COLLISIONRGBA [COLLISIONRGBA ...]
                        The color of the collision meshes, if they exist
```

## Examples

Go to `../../build/multiverse/modules/multiverse_parser` and run `ctest`. The scene graph from [`../../tests/multiverse_parser/input`](https://github.com/Multiverse-Framework/Multiverse/tree/ICRA-2024/multiverse/tests/multiverse_parser/input) will be translated in the `output` folder in [`../../tests/multiverse_parser`](https://github.com/Multiverse-Framework/Multiverse/tree/ICRA-2024/multiverse/tests/multiverse_parser).
