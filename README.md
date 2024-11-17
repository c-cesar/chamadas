# Protótipo de um site que agregue as chamadas de artigos para revistas científicas.

Este projeto utiliza [Hades](https://github.com/kitallis/hades) e [Zola](https://www.getzola.org/).

Para adicionar fontes basta editr o arquivo chamadas.toml seguindo o modelo.

```
[[authors]]
name = "Temporalidades - UFMG"
feed = "https://periodicos.ufmg.br/index.php/temporalidades/gateway/plugin/WebFeedGatewayPlugin/rss2"
tag = ["UFMG", "História"]
```

Se você quiser rodar uma cópia, deve instalar o Hades e executar

```
hades -c chamadas.toml
```

Isso vai povoar a pasta `site/conent` para o Zola. Para gerar o site é preciso executar o zola com:

```
zola build
```

Isso vai povoar a pasta `public` com arquivos HTML. Estes arquivos devem ser expostos para um servidor de arquivos estáticos.
