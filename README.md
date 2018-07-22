# Tutorial

Esta aplicação foi desenvolvida seguindo 
 [esse tutorial](https://coursetro.com/posts/code/154/Angular-6-Tutorial---Learn-Angular-6-in-this-Crash-Course).

# Build de produção

Disponivel para uso em: [http://yuri8p.github.io/ng6/](http://yuri8p.github.io/ng6/)

Para fazer o deploy no github pages de uma aplicação Angular que utiliza rotas é necessário fazer o seguinte:

1. Gerar o build de produção especificando:
    - `--prod` para gerar arquivos de produção menores; 
    - `--base-href` com o **/nome-do-repositorio/** entre barras;
    - `--output-path` como **docs** para facilitar a configuração do github pages;
    - Exemplo: `ng build --prod --output-path docs --base-href /ng6/`
2. Fazer uma cópia do `docs/index.html` como `docs/404.html` para que as rotas funcionem em servidores estáticos.
3. Configurar o `Source` do `Github Pages` como `master branch /docs folder` nas configurações do seu repositório. **https://github.com/seu_usuario/repositorio/settings**
4. Salvar as configurações e acessar a url do projeto no Github Pages.

# Screenshot

![](screenshot.png)
