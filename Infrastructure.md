# Servers

* summer.brightway.dev - 176.9.61.115
* spring.brightway.dev - 5.9.116.7
* winter.brightway.dev - 176.9.26.123

# Environments

Make conda work online:

    source /opt/tljh/user/etc/profile.d/conda.sh

Make environments available:

    sudo conda install nb_conda_kernels

List environments:

    conda info --envs

Remove an environment:

    sudo conda remove --name <name> --all

It is much easier to just nuke environments than adding packages to them.

Conference

    sudo conda create -n conference -c conda-forge -c cmutel brightway25 bw2data">=4.0.dev28" ipykernel ipycytoscape nbformat plotly matplotlib pandas jupyterlab-plotly-extension

**Note**: The `ipycytoscape` library also has to be installed in base conda environment or you get Javascript nightmares when using remote servers.

    sudo conda install ipycytoscape

pyecospold

    sudo conda create -n pyecospold -c conda-forge -c cmutel ipykernel pyecospold pyilcd

Premise:

    sudo conda create -n premise -c conda-forge -c cmutel -c romainsacchi premise"==2023.09.11" brightway2"==2.4.3" ipykernel

bw2extdb

    sudo conda create -n bw2extdb -c conda-forge -c cmutel brightway2 ipykernel pip sqlmodel psycopg2-binary streamlit
    sudo pip install git+https://github.com/Blowgren/bw2extdb@main

llm

    sudo conda create -n llm -c conda-forge ipykernel langchain"==0.0.288" openai"==0.28.0" pandas tiktoken matplotlib tqdm chromadb"==0.4.10"

## libmamba

Make mamba the default solver for conda package management:

    sudo conda update conda
    sudo conda install -n base conda-libmamba-solver
    sudo conda config --set solver libmamba

# nbgitpuller

## Spring

`[Click here to install conference materials](https://spring.brightway.dev/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDepart-de-Sentier%2Fbrightcon-2023-talks&urlpath=lab%2Ftree%2Fbrightcon-2023-talks%2F)`

## Winter

`[Click here to install conference materials](https://winter.brightway.dev/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDepart-de-Sentier%2Fbrightcon-2023-talks&urlpath=lab%2Ftree%2Fbrightcon-2023-talks%2F)`

## Summer

`[Click here to install conference materials](https://summer.brightway.dev/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FDepart-de-Sentier%2Fbrightcon-2023-talks&urlpath=lab%2Ftree%2Fbrightcon-2023-talks%2F)`
