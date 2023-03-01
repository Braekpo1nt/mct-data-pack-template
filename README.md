# MCT Data Pack Template
This template is designed to be used for new MCT Data Packs. Data Packs for MCT have to be able to communicate to each other, so there are a few rules to follow, outlined below.

## Using this Template
To use this template, follow GitHub's own instructions on [creating a repository from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

- Go to the [homepage of this repository](https://github.com/Braekpo1nt/mct-data-pack-template)
- Select **Use this template**
- Choose **Create a new repository**
- Configure the repository as normal
- Click **Create repository from template**
- Follow the instructions in the template repository's [Getting Started](#getting-started) section to fill out the boiler plate items, rename folders, and initialize the repository.


## Getting Started
- Rename the [data/mct-template/](data/mct-template/) directory to `mct-<THE NAME OF THIS REPOSITORY>`
    - e.g. `mct-hub` or `mct-score-manager`
    - > Important: this folder must be lowercase
- Change `mct-template` to match the name of the folder you just renamed above in both [data/minecraft/tags/functions/load.json](data/minecraft/tags/functions/load.json) and [data/minecraft/tags/functions/tick.json](data/minecraft/tags/functions/tick.json)
- Fill in the description of [pack.mcmeta](pack.mcmeta)
- Go to the **Projects** tab of your new repository and link the project to the [MCT Project](https://github.com/users/Braekpo1nt/projects/2/views/1)
- Add a link to the new Data Pack repository to the [MCT Project](https://github.com/users/Braekpo1nt/projects/2/views/1) `README.md`
- Replace the contents of this [README.md](README.md) file with [README-TEMPLATE.md](README-TEMPLATE.md), and fill in the italicized parts with information about the Data Pack and how to use it
- Delete [README-TEMPLATE.md](README-TEMPLATE.md)

## Requirements
You must follow these rules to maintain compatibility across MCT data packs:

- The folder with the `function/` directory must start with `mct-`, match the name of your repository, and be all lowercase. 
    - That way it's easy to keep track of when `/function` commands are trying to use other Data Pack's `.mcfunction`s.
- Ensure your scoreboard names are unique across MCT Data Packs. Otherwise there will be conflicts.
- Describe the purpose of every `.mcfunction` file in a comment at the top
    - use the `#` character at the start of a line to make it a comment


