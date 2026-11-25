# kelmedev.github.io

> Repositório de GitHub Pages preparado para receber um site pessoal com domínio próprio.

**Tipo:** Projeto pessoal · 2025

## Sobre

**Função:** o repositório contém apenas a configuração de publicação no GitHub Pages: um arquivo `CNAME` com o domínio personalizado, este README e a licença.

**Objetivo:** deixar a hospedagem pronta para um site pessoal. Ainda não há páginas (nenhum `index.html`), então o conteúdo do site não foi feito.

## Como funciona o GitHub Pages aqui

- **Fonte de publicação:** branch `main`, pasta raiz (`/`), no modo clássico (sem workflow do Actions).
- **Domínio próprio:** o GitHub Pages lê o domínio escrito no arquivo `CNAME` e passa a responder por ele.
- **Conteúdo atual:** sem `index.html`, o Pages usa o `README.md` como página inicial (o Jekyll converte o Markdown em HTML).
- **Nome do repositório:** apesar do formato `nome.github.io`, o dono é `itskelme`, então este é um site de projeto, não o site de usuário (que exigiria o nome `itskelme.github.io`). Com domínio próprio configurado, isso não muda o endereço final.

Para o domínio funcionar, o DNS dele precisa apontar para o GitHub Pages:

| Registro | Nome | Valor |
| --- | --- | --- |
| `A` | `@` | `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153` |
| `AAAA` (opcional) | `@` | `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153` |
| `CNAME` (opcional) | `www` | `itskelme.github.io` |

Depois que o DNS propagar, vale ativar "Enforce HTTPS" em *Settings > Pages*.

## Estrutura do projeto

| Caminho | Descrição |
| --- | --- |
| `CNAME` | Domínio personalizado do GitHub Pages. Não remova nem renomeie. |
| `README.md` | Este arquivo; também é a página inicial enquanto não houver `index.html` |
| `LICENSE` | Licença CC BY-NC 4.0 |

## Como publicar conteúdo

1. Adicione um `index.html` (ou um site Jekyll) na raiz da branch `main`.
2. Faça push. O GitHub Pages reconstrói o site sozinho em alguns minutos.
3. Mantenha o `CNAME` na raiz para não perder o domínio.

## Referências

- [Sobre o GitHub Pages](https://docs.github.com/pt/pages/getting-started-with-github-pages/about-github-pages)
- [Gerenciar um domínio personalizado](https://docs.github.com/pt/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)
- [Proteger o site com HTTPS](https://docs.github.com/pt/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https)

## Autores

- Diego Kelme Santos da Silva — [@itskelme](https://github.com/itskelme)

## Licença

Este projeto está sob a licença [CC BY-NC 4.0](LICENSE): uso pessoal e modificação permitidos com atribuição; uso comercial proibido.
