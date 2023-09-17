# Servers

* summer.brightway.dev - 176.9.61.115
* spring.brightway.dev - 5.9.116.7
* winter.brightway.dev - 176.9.26.123

# Environments

List environments:

    conda info --envs

Remove an environment:

    sudo conda remove --name <name> --all

It is much easier to just nuke environments than adding packages to them.

Conference

    sudo conda create -n conference -c conda-forge -c cmutel brightway25 bw2data"==4.0.dev21" ipykernel ipycytoscape

**Note**: The `ipycytoscape` library also has to be installed in base conda environment or you get Javascript nightmares.

Premise:

    sudo conda create -n premise -c conda-forge -c cmutel -c romainsacchi premise"==2023.09.11" brightway2"==2.4.3" ipykernel

Conference

    sudo conda create -n conference -c conda-forge -c cmutel brightway25 bw2data"==4.0.dev21" ipykernel ipycytoscape plotly pandas

## libmamba

Make mamba the default solver for conda package management:

    sudo conda update conda
    conda install -n base conda-libmamba-solver

# nbgitpuller

## Spring

`[Click here to install conference materials](https://spring.brightway.dev/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDepart-de-Sentier%2Fbrightcon-2023-talks&urlpath=lab%2Ftree%2Fbrightcon-2023-talks%2F)`

## Winter

`[Click here to install conference materials](https://winter.brightway.dev/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDepart-de-Sentier%2Fbrightcon-2023-talks&urlpath=lab%2Ftree%2Fbrightcon-2023-talks%2F)`

## Summer

`[Click here to install conference materials](https://summer.brightway.dev/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDepart-de-Sentier%2Fbrightcon-2023-talks&urlpath=lab%2Ftree%2Fbrightcon-2023-talks%2F)`
