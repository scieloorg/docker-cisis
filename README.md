# Docker-Cisis

Docker para execução de comandos CiSIS

### Contruir a imagem:

```docker build -t cisis_image . ```

### Rodando o conteiner da image utilizando a opção **-t** (pseudo terminal):

```docker run -t -d --name cisis_container cisis_image```

### Acessando o conteiner (sh):

```docker exec -ti  cisis_container sh```

### Rodando um comando CISIS:

```docker exec -ti cisis_container mx```

## Rodando o conteiner da image configurando volume:

```docker run -t -d -v cisis:/cisis --name cisis_container cisis_image```
