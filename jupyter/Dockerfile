FROM jupyter/datascience-notebook:latest

RUN pip install --upgrade pip
RUN pip install \
    black \
    jupyter-lsp \
    jupyterlab_code_formatter \
    jupyterlab-git \
    python-language-server[all]
RUN jupyter labextension install \
    @jupyterlab/git \
    @jupyterlab/toc \
    @krassowski/jupyterlab-lsp \
    @lckr/jupyterlab_variableinspector \
    @mohirio/jupyterlab-horizon-theme \
    @ryantam626/jupyterlab_code_formatter
RUN jupyter serverextension enable --py \
    jupyterlab_code_formatter \
    jupyterlab_git
