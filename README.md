# 20190912-data-analytics-timeseries
Materials for the Conclusion &amp; AMIS Machine Learning Guild - MeetUp on Data Analytics and Time Series

To get started on the workshop - go through these steps:

Run a command line shell on a Docker host

Execute this command to run a Jupyter Notebook (see https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-scipy-notebook for more details on this Container Imgage that has Python 3.x, Anaconda, Pandas, Jupyter Lab, git)

`docker run --name timeseries-data-analytics -d -p=8888:8888 jupyter/scipy-notebook`

When the container is running, inspect its logs - and locate the Jupyter Lab token (after the line:  *The Jupyter Notebook is running at:*)
`docker logs timeseries-data-analytics --follow`

To complete setting up the container, please execute this command to open a shell session inside the container:

`docker exec -it  base-timeseries  /bin/bash`

then - inside the container - execute: 

`git clone https://github.com/AMIS-Services/20190912-data-analytics-timeseries`

this clones a GitHub Repo that contains the notebook *environment-setup*. This notebook should be executed from the browser as a regular Jupyter Notebook. Then, open Notebook in the browser:

http://IP-Docker-Host:8888/notebooks/environment-setup.ipynb

and run the Notebook. This will install the required Python Libraries and the GitHub Repositories for the workshop.
