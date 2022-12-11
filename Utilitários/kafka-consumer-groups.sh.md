***
* **Todos os grupos**
```
bin/kafka-consumer-groups.sh --all-groups --bootstrap-server localhost:9092 --describe
```
* **Grupo específico**
```
bin/kafka-consumer-groups.sh --group <nome_grupo> --bootstrap-server localhost:9092 --describe
```