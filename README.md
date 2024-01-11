# commandblocks

This repository compiles command block setups and commands designed for Minecraft Java. The goal is to consolidate scattered command block configurations and commands into a unified platform, eliminating the need to sift through countless threads on the internet and random YouTube videos.

## Contents

### Scoreboards

* [Display a scoreboard within a given range.](./src/scoreboards/DISPLAY_WITHIN_RANGE.md)

## Contributing

If you would like to contribute to this repository, please follow the guidelines below.

### Adding a new snippet

1. Create a new file in the matching directory under `src/`. 
    The file name should be the name of the snippet in all caps, with underscores instead of spaces. For example, if the snippet name is "Display a scoreboard within a given range", the file name should be `DISPLAY_WITHIN_RANGE.md`.

2. Add the following to the top of the file:

    ```markdown
    # <Snippet name>

    <Description>

    ## Setup

    <Setup instructions>

    ## Command blocks

    <Command block instructions>
    ```

3. Add the following to the contents section of this README:

    ```markdown
    * [<Snippet name>](./src/<Snippet directory>/<Snippet file name>)
    ```
