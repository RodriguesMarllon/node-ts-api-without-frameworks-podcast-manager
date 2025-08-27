# Podcast Manager

### Descrição
Um app ao estilo netflix, onde eu possa centralizar diferentes episódios de podcasts separados por categoria

### Domínio
Podcasts feitos em vídeo

### Features
- Listar os eposódios podcasts em sessões de categorias
    - Saúde, bodybuilder, mentalidade, humor
- Filtrar episódios por nome de podcast

## Como

### Feature
- Listar os eposódios podcasts em sessões de categorias

### Como vou implementar:

GET: retorna lista de episódios

```js
[

    {
        podcastName: "flow",
        episode: "CBUM - Flow #319",
        videoId: "pQSuQmUfS30",
        category: ["saúde", "bodybuilder"]
    },
    {
        podcastName: "flow",
        episode: "RUBENS BARRICHELLO - Flow #339",
        videoId: "4KDGTdiOV4I",
        category: ["esporte", "corrida"]
    },
]
```

GET: retorna a lista de episódios baseado em um parametro enviado pelo cliente do nome do podcast