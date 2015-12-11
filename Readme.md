Apache Giraph Dev-in-box
============================================


This is a dev-in-box for Apache Giraph.

```bash
vagrant up
```


### How to use?

1. You can develop your regular java aapplication and make a jar file. Then you can put it under ```dib/``` folder.
2. ```vagrant ssh```
3. ```docker ps```
4. ```docker exec -it <container_id> "/bin/bash"```
5. ```cd /vagrant```
6. ```$HADOOP_HOME/bin/hadoop jar <youjar>.jar org.apache.giraph.GiraphRunner mypackage.DummyComputation --yarnjars <your>.jar --workers 1 --vertexInputFormat org.apache.giraph.io.formats.JsonLongDoubleFloatDoubleVertexInputFormat --vertexInputPath /user/root/input/tiny-graph.txt -vertexOutputFormat org.apache.giraph.io.formats.IdWithValueTextOutputFormat --outputPath /user/root/dummy-output```
7. Your output will be in /user/root/dummy-output on the hdfs file system ``` $HADOOP_HOME/bin/hadoop dfs -cat /user/root/dummy* | less```


### Detailed description
Coming soon.
