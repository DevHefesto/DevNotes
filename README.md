# Documentação HTML

## Texto

- `<h1> <h2> ... <h6>`: Cria títulos e a cada número gera subtítulos com menos negrito e fonte menor, ou seja, menos destaque.

- `<p>`: Cria um parágrafo.

- `<br>`: Quebra de linha.

- `<hr>`: Cria uma linha reta separadora cobrindo toda a largura da página.

## Imagens

- `<a href="Link" alt="Texto clicável, o qual irá levar ao link">`: Ancora um link.

- `<img src="Especifíca o diretório" alt="Texto alternativo em caso de não carregamento da imagem">`: Referencia uma imagem.

- `<figure>`: Indica elementos relacionados a gráficos, imagens e ilustrações.

- `<figcaption>`: Texto relacionado à imagem referenciada com o anchor (`<a>`).

## Semântica

- `<header>`: Define o cabeçalho do site ou de uma seção e, normalmente, contém elementos como logo e menu de navegação.

- `<nav>`: Define um conjunto de links de navegação ou menu.

- `<section>`: Define uma seção no documento.

- `<aside>`: Define um local para conteúdo além do principal, como uma barra lateral.

- `<footer>`: Define o rodapé do documento.

## Vídeos

- `<video controls>`: É usada para incorporar e reproduzir vídeos.
    - O atributo controls é adicionado para exibir os controles padrão do player, como play, pause e controle de volume.

- `<source src="Especifíca o diretório" type="Especifíca o tipo do vídeo">`: É usada dentro da tag `<video>` para especificar os diferentes formatos de vídeo a serem oferecidos.

## Listas

- `<ul>`: Representa unordered list, ou seja, listas não ordenadas.

- `<ol>`: Representa ordered list, ou seja, listas ordenadas.

- `<dl>`: Representa description list, ou seja, listas de descrição.
    - Exemplo de lista ordenada e não ordenada:
        ```html
        <ul>
            <li>Primeiro item</li>
            <li>Segundo item</li>
            <li>Terceiro item</li>
        </ul>

        <ol>
            <li>Primeiro item</li>
            <li>Segundo item</li>
            <li>Terceiro item</li>
        </ol>
        ```
    - Exemplo de lista de descrição:
        ```html
        <dl>
            <dt>Primeiro item</dt>
            <dd>- Descrição do primeiro item</dd>
            <dt>Segundo item</dt>
            <dd>- Descrição do segundo item</dd>
        </dl>
        ```

- `<select>`: Cria caixas de seleção e listas suspensas.
    - OBS: Deve utilizar a tag `<option>` para definir as opções disponíveis na lista.
    - Exemplo de lista suspensa:
        ```html
        <select>
            <option value="opcao1">Opção 1</option>
            <option value="opcao2">Opção 2</option>
            <option value="opcao3">Opção 3</option>
        </select>
        ```
