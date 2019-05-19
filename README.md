
# pdnd-open-notebooks

  

### INFO

  

This repo contains a set of notebooks devoloped using [pdnd-nteract](https://github.com/teamdigitale/daf-nteract) on top of a [datascience docker image](https://github.com/jupyter/docker-stacks/tree/master/datascience-notebook) provided by [jupyter project](https://jupyter.org/). The image contains a ready to use datascience environment with the most used datascience libraries for **python3**, **R**, and **Julia**. If you want to deepen about the set of libraries you can read [this](https://jupyter-docker-stacks.readthedocs.io/en/latest/). 

[Pdnd-nteract](https://github.com/teamdigitale/daf-nteract) is a customisation of [nteract](https://nteract.io/) that allows users registered into the [pdnd](https://dataportal.daf.teamdigitale.it/) to search and load datasets into the notebook from about 7000 italians public datasets. If you want to know more about the project you can start from [here](https://github.com/teamdigitale/daf-nteract).  Some material to understand how it works can be:

 - TODO Medium post still draft
 - [Video tutorial](https://www.youtube.com/watch?v=nlZnYcz66YE)
 - [Tutorial](open-notebooks-example/tutorial.ipynb) in this repo
 - [Examples](open-notebooks-example/) in this repo

### GETTING STARTED

[Docker](https://www.docker.com/) MUST be installed on your local machine

TODO change image with the datascience 

From [dockerhub](https://hub.docker.com/r/teamdigitale/daf-nteract)

```
git clone git@github.com:teamdigitale/pdnd-open-notebooks.git
cd pdnd-open-notebooks
docker pull teamdigitale/daf-nteract
docker run -p 8888:8888 -v "$PWD":/home/jovyan/work daf-nteract
```
Save the token from the output of your console as:
http://(b4fd9e3ef290 or 127.0.0.1):8888/?token=XXXXXXXXXXXXXX
and open your browser at [http://localhost:8888]. If you are asked the token paste it.

You should see something like this:
![start](https://raw.githubusercontent.com/teamdigitale/pdnd-open-notebooks/master/img/start.png)

CONGRATULATIONS NOW YOU ARE READY TO CONTRIBUTE.

### HOW TO CONTRIBUTE
Never made an open source contribution before?


1.  Fork this repository to your local GitHub organization.

2.  Clone the repository to your local machine using:

```
$ git clone https://github.com/github-username/repository-name.git
```

3.  Install the image as in the steps described above

5.  Create a new branch for your new notebook using:

```
$ git checkout -b branch-name-here
```

6.  Create a new analysis with one of the kernel on some public data provided by the platform

7.  Add and commit the changed files using `git add` and `git commit`.

8. Push the changes to the remote repository using:

```
$ git push origin branch-name-here
```

9. Submit a pull request to the upstream repository.

10. Title the pull request per the requirements outlined in the section below.

11. Set the description of the pull request with a brief description of what you did and any questions you might have about what you did.

12. Wait for the pull request to be reviewed by a maintainer.

13. Make changes to the pull request if the reviewing maintainer recommends them.

14. Celebrate your success after your pull request is merged! :tada: