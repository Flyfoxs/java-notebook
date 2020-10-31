
# Usage

```
docker run -dt -p 8888:8888  --name java_notebook \
            --volume=$(pwd)/notebook:/home/jovyan/notebook \
            --volume=$(pwd)/.jupyter:/home/jovyan/.jupyter \
            --volume=${HOME}/.m2:/home/jovyan/.m2 \
            --volume=${HOME}/.ivy2:/home/jovyan/.ivy2 \
            -e  TZ=Asia/Shanghai \
            jbindinga/java-notebook


docker exec -it -u root  java_notebook bash

```


# Ref
https://github.com/jbindinga/java-notebook

https://github.com/SpencerPark/IJava
