# Lab HDFS - API Hadoop

## Applications
- **HadoopFileStatus** : Infos fichiers + renommage
- **ReadHDFS** : Lecture fichiers HDFS  
- **WriteHDFS** : Écriture fichiers HDFS

## Commandes
```bash
# Démarrer cluster
docker start hadoop-master hadoop-slave1 hadoop-slave2
docker exec -it hadoop-master bash
./start-hadoop.sh

# Compiler
mvn clean package

# Exécuter
hadoop jar HadoopFileStatus.jar /input/file.txt new_name.txt
hadoop jar ReadHDFS.jar file.txt
hadoop jar WriteHDFS.jar /output/file.txt
```
Structure
```
src/main/java/edu/supmti/hadoop/
├── HadoopFileStatus.java
├── ReadHDFS.java
└── WriteHDFS.java
```
"# BIGDATA_lab1_Programmation-avec-API" 
