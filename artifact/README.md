# Projects Artifacts

# Loading the docker image

Download the file from URL, then load the docker image using the command below:



```bash
cat rep-lra-part-* > rep-lra.tar
docker load --input lra_image.tar

docker run --rm  --gpus all -v ${PWD}:/workspace -it lra_image bash

# inside the container, run 

. ./artifact/scripts/train.sh

```
