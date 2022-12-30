***
O Docker pode construir imagens automaticamente lendo as instruções de um Dockerfile. 
Um Dockerfile é um documento de texto que contém todos os comandos que um usuário poderia chamar na linha de comando para montar uma imagem. 
Usando o Docker build os usuários podem criar um build automatizado que executa várias instruções de linha de comando em sucessão.

***
Lista de instruções no Dockerfile:

-   `ADD`
-   `COPY`
-   `ENV`
-   `EXPOSE`
-   `FROM`
-   `LABEL`
-   `STOPSIGNAL`
-   `USER`
-   `VOLUME`
-   `WORKDIR`
-   `ONBUILD`

***
**Multi-stage builds** 
Com construções em várias etapas, você usa várias declarações FROM em seu Dockerfile. Cada instrução FROM pode usar uma base diferente, e cada uma delas começa uma nova etapa da construção. Você pode copiar seletivamente artefatos de um estágio para outro, deixando para trás tudo o que você não quer na imagem final.

**Exemplo:**

```
FROM golang:1.16 AS builder
WORKDIR /go/src/github.com/alexellis/href-counter/
RUN go get -d -v golang.org/x/net/html  
COPY app.go    ./
RUN CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o app .

FROM alpine:latest  
RUN apk --no-cache add ca-certificates
WORKDIR /root/
COPY --from=builder /go/src/github.com/alexellis/href-counter/app ./
CMD ["./app"]
```


