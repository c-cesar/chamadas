# Chamadas

Este é um protótipo de site que agregue chamadas de artigos para revistas científicas. Ele cadastra o RSS de notícias das revistas e mostra as publicações aqui. Versão de testes em execução em https://chamadas.masdivago.cc

Este projeto utiliza [Hades](https://github.com/kitallis/hades) e [Zola](https://www.getzola.org/).

Para adicionar fontes basta editar o arquivo `chamadas.toml` seguindo o modelo.

```
[[authors]]
name = "Boletim do Tempo Presente"
feed = "https://periodicos.ufs.br/tempopresente/gateway/plugin/AnnouncementFeedGatewayPlugin/rss2"
tags = ["UFS", "História"]
```

É possível editar o arquivo pelo próprio site do GitHub, sem precisar usar a linha de comando.
