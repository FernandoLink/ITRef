***
* **Criar tópico no kafka**
```
bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1 --topic <nome_topico>
```
* **Lista tópicos**
```
bin/kafka-topics.sh --list --bootstrap-server localhost:9092
```
* **Descreve os tópicos**
```
bin/kafka-topics.sh --describe --bootstrap-server localhost:9092
```
* **Alterar tópico com 3 partições**
```
bin/kafka-topics.sh --alter --bootstrap-server localhost:9092 --topic ECOMMERCE_NEW_ORDER --partitions 3 
```