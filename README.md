# README

This is a docker image for [http://pencil.evolus.vn/](http://pencil.evolus.vn/).

# Running

```terminal
% docker run \
    --detach=false \
    -it \
    --rm \
    -e DISPLAY=unix$DISPLAY \
    -e GDK_DPI_SCALE \
    -e GDK_SCALE \
    -v /etc/localtime:/etc/localtime:ro \
    -v ${HOME}:/${USER} \
    -v /tmp/.X11-unix:/tmp/.X11-unix \
    dmitryrck/pencil
```
