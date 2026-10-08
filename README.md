# BrisaShop

Superprojeto Git do BrisaShop, loja online fictícia de uma varejista de moda que vende roupas, calçados e acessórios. É o ponto de entrada do sistema: a documentação e cada microsserviço têm repositório próprio, e este os reúne como submódulos Git.

| Pasta | Repositório | Conteúdo |
|---|---|---|
| `docs/` | [brisashop-docs](https://github.com/sidartaoss/brisashop-docs) | Documentação de arquitetura, mantida como código |
| `microservices/brisashop-ordering/` | [brisashop-ordering](https://github.com/sidartaoss/brisashop-ordering) | Pedidos: a jornada de compra, da sacola à criação do pedido |

Novos microsserviços entram como submódulos em `microservices/`.

## Como clonar

```bash
git clone --recurse-submodules https://github.com/sidartaoss/brisashop.git
```

Em um clone feito sem `--recurse-submodules`, o comando `git submodule update --init` baixa os submódulos. Cada um fica no commit registrado pelo superprojeto; para trabalhar nele, basta entrar na pasta e trocar para a branch `main`.
