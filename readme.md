# Usage

* 开启容器

```
git clone git@github.com:Flyfoxs/java-notebook.git
cd java-notebook
docker run -dt -p 8888:8888 -p 7000-7005:7000-7005 --name java_notebook \
            --volume=$(pwd)/notebook:/home/jovyan/notebook \
            --volume=$(pwd)/.jupyter:/home/jovyan/.jupyter \
            --volume=${HOME}/.m2:/home/jovyan/.m2 \
            --volume=${HOME}/.ivy2:/home/jovyan/.ivy2 \
            -e  TZ=Asia/Shanghai \
            --restart always \
            jbindinga/java-notebook

```

* 访问 Jupyter notebook
Link:  http://localhost:8888,  Password: felix.lilao




# Java Example
* [单例](./notebook/singleton.ipynb)
* [Spring book(Hello world)](./notebook/springboot_tomcat.ipynb)
* [Stream (Hello world)](./notebook/stream.ipynb)
* [Spring 配置文件优先级](./notebook/springboot_conf_priority.ipynb)
* [垃圾回收-弱引用](./notebook/weakReference.ipynb)



# Ref

https://github.com/jbindinga/java-notebook

https://github.com/SpencerPark/IJava
