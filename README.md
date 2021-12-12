# ls3-playground
A python playground for the LineScale 3
Made by Mark Koh

## Running
To run the jupyter-lab docker image and mount the repo data into the container run the following command
```bash
docker run \
  -p 8888:8888 \
  --user root \
  -w /home/$USER \
  -v $(pwd):/home/$USER \
  -e NB_USER=$USER \
  -e NB_UID=$UID \
  -e CHOWN_HOME=yes \
  jupyter/scipy-notebook
```

