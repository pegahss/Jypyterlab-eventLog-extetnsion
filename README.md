# Jypyterlab-eventLog-extetnsion

#Run this command to create a new environment named jupyterlab-logEvent-Ext

conda create -n jupyterlab-logEvent-Ext --override-channels --strict-channel-priority -c conda-forge -c nodefaults jupyterlab=3 cookiecutter nodejs jupyter-packaging git

#Run these commands to activate the jupyterlab-ext environment and start JupyterLab in your default web browser.

conda activate jupyterlab-logEvent-Ext

# Build and install the extension for development

#Clone the repo to your local environment

#Change directory to the jupyterlab-logEvent-Ext

#Install package in development mode

pip install -e .

#Link your development version of the extension with JupyterLab

jupyter labextension develop . --overwrite

#Run JupyterLab in another terminal
jupyter lab



You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.

#Watch the source directory in one terminal, automatically rebuilding when needed

jlpm run watch

#Rebuild extension Typescript source after making changes

jlpm run build




if you grt any error on importing library/dependencies, you will need to install these dependencies. Run the following commands in the repository root folder to install the dependencies and save them to your package.json:

jlpm add 'dependensies-name' 

example : jlpm add @jupyterlab/apputils





