# rpgmaker-script-skeleton

## Overview

A simple skeleton app for RPG Maker scripts. The idea is that scripts can be developed independent of RPG Maker and later exported and integrated in the actual app.

By developing RPG Maker scripts outside of RPG Maker, tests can take advantage of the many tools/workflows used for professional Ruby development, such as:
- Advanced code editors
- Unit & functional testing
- Continuous integration
- Code quality metrics
- Gem/package management

When a new version of the script is released, a task can be run to build all code into a single Ruby file then upload it somewhere that a game could download or otherwise consume at runtime.
