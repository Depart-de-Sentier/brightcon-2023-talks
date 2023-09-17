# Environments

List environments:

    conda info --envs

Remove an environment:

    sudo conda remove --name <name> --all

It is much easier to just nuke environments than adding packages to them.

Premise:

    sudo conda create -n premise -c conda-forge -c cmutel -c romainsacchi premise"==2023.09.11" brightway2"==2.4.3" ipykernel

Conference

    sudo conda create -n conference -c conda-forge -c cmutel brightway25 bw2data"==4.0.dev21" ipykernel ipycytoscape plotly pandas

## libmamba

Make mamba the default solver for conda package management:

    sudo conda update conda
    conda install -n base conda-libmamba-solver

# nbgitpuller

Replace `spring` with the correct server.

[Brightcon 2023](https://spring.brightway.dev/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDepart-de-Sentier%2Fbrightcon-2023-talks&urlpath=lab%2Ftree%2Fbrightcon-2023-talks%2F)
