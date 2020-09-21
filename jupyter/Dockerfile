FROM jupyter/datascience-notebook:latest

RUN pip install --upgrade pip
RUN pip install \
    black \
    ipympl \
    jupyter-lsp \
    jupyterlab_code_formatter \
    jupyterlab-git \
    python-language-server[all]
RUN jupyter labextension install \
    @ijmbarr/jupyterlab_spellchecker \
    @jupyter-widgets/jupyterlab-manager \
    @jupyterlab/git \
    @jupyterlab/toc \
    @krassowski/jupyterlab_go_to_definition \
    @krassowski/jupyterlab-lsp \
    @lckr/jupyterlab_variableinspector \
    @mohirio/jupyterlab-horizon-theme \
    @ryantam626/jupyterlab_code_formatter \
    jupyterlab_filetree
RUN jupyter serverextension enable --py \
    jupyterlab_code_formatter \
    jupyterlab_git
