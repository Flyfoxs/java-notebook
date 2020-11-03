
# Usage

```
docker run -dt -p 8888:8888 -p 7000-7005:7000-7005 --name java_notebook \
            --volume=$(pwd)/notebook:/home/jovyan/notebook \
            --volume=$(pwd)/.jupyter:/home/jovyan/.jupyter \
            --volume=${HOME}/.m2:/home/jovyan/.m2 \
            --volume=${HOME}/.ivy2:/home/jovyan/.ivy2 \
            -e  TZ=Asia/Shanghai \
            jbindinga/java-notebook

```

# Jupyter notebook
Link:  http://localhost:8888

Password: felix.lilao

# Ref
https://github.com/jbindinga/java-notebook

https://github.com/SpencerPark/IJava
