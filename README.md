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
        
## Tabelas

- `<table>`: Cria tabela para organizar dados.
- `<tr>`: Dispõe as tags `<td>` em linha.
- `<td>`: Dispõe as células (conteúdos) da tabela.
- `<th>`: Cabeçalho da tabela. Centraliza e coloca em negrito seu conteúdo.

  Ex:
  ```html
  <table>
    <tr>
      <th>Coluna 1</th>
      <th>Coluna 2</th>
      <th>Coluna 3</th>
    </tr>
    <tr>
      <td>Conteúdo 1</td>
      <td>Conteúdo 2</td>
      <td>Conteúdo 3</td>
    </tr>
  </table>
    ```
  ## Semântica de Tabelas

- `<caption>`: Define qual será o conteúdo da tabela.

- `<thead>`: Define o cabeçalho da tabela. Deve envolver os conteúdos de `<th>`.

- `<tbody>`: Define o corpo da tabela, semelhante ao `<body>`.

- `<tfoot>`: Define o rodapé da tabela, semelhante ao `<footer>`.

  Ex:
  ```html
  <table>
    <thead>
      <tr>
        <th>Coluna 1</th>
        <th>Coluna 2</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Conteúdo coluna 1 linha 1</td>
        <td>Conteúdo coluna 2 linha 1</td>
      </tr>
      <tr>
        <td>Conteúdo coluna 1 linha 2</td>
        <td>Conteúdo coluna 2 linha 2</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <td>Conteúdo coluna 1 linha 3</td>
        <td>Conteúdo coluna 2 linha 3</td>
      </tr>
    </tfoot>
  </table>
  ```
  ## Formulários
  
- `<form>`: Contêiner para diferentes tipos de campos de entrada de dados, tais como: campos de texto, caixas de seleção, botões de opção, botões de envio, etc.

- `<form action="">`: Define recebe como valor o destino dos dados que serão submetidos no formulário, que, normalmente é uma página em uma linguagem de backend como PHP, Java, ASP, etc.

- `<form action="" target="">`: O atributo target especifica onde exibir a resposta recebida após o envio do formulário, como por exemplo `_blank` (em uma nova janela), `_self` (na janela atual), `_parent` (no quadro pai), `_top` (em todo o corpo da janela) ou `framename` (em um iframe nomeado).

- `<form action="" method="">`: O atributo method especifica o método HTTP a ser usado ao enviar os dados do formulário, que podem ser POST, anexando os dados do formulário à URL ou GET, que anexa os dados do formulário dentro do corpo da solicitação HTTP.

Tipos de campos para envio de dados

- `<input type="text">`: Exibe um campo de entrada de texto de uma linha.

- `<input type="radio">`: Exibe um botão para cada item de uma série de opções, onde somente um item pode ser selecionado.

- `<input type="checkbox">`: Exibe uma caixa de seleção para cada item de uma série de opções, onde pode-se selecionar mais de um item.

- `<input type="submit">`: Exibe um botão enviar (para submeter o formulário).

- `<input type="button">`: Exibe um botão clicável.

- `<input type="date">`: Exibe (ao clicar no campo) um calendário para selecionar uma data.

- `<input type="email">`: Exibe um campo para entrada de um endereço de e-mail. O valor de entrada é validado automaticamente para garantir que seja um endereço de e-mail formatado corretamente.

Outro campo muito utilizado é a lista suspensa, que é definida pelo elemento `<select>` seguido das opções da lista, definidas pelos elementos `<option>`.
Ex:
```html
<select id="carros" name="carros">
  <option value="gol">Gol</option>
  <option value="palio">Pálio</option>
  <option value="hb20">HB20</option>
  <option value="clio">Clio</option>
</select>
```
OBS: Adicione o atributo selected dentro da tag option para que aquela opção apareça já selecionada em sua lista suspesa.
Ex: `<option value=“gol” selected >Gol</option>`

Todo campo do formulário deve ter um atributo name que deverá receber o nome do campo (sem espaços) para que o servidor possa pegar o valor enviado.

Para atribuir um rótulo ao campo, utiliza-se o elemento `<label>`. É importante a utilização deste elemento para que leitores de tela identifiquem o campo para pessoas com deficiência visual. Este elemento ajuda os usuários que têm dificuldade em clicar em regiões muito pequenas pois ao clicar no texto do <label>, ele seleciona o campo, mas, para isso, é necessário utilizar o atributo for, que deve receber o mesmo valor do atributo id do campo a que se refere, como no exemplo a seguir:

`<label for=“linguagem”>`Digite aqui a sua linguagem favorita`</label>`

`<input type=“text” id=“linguagem” name=“linguagemFavorita”>`

Abaixo um exemplo de formulário com campos de entrada de texto para nome e sobrenome. Veja que comumente, os valores dos atributos for, id e name são iguais.

```HTML
<form>
        <label for=“nome”>Nome</label><br>
        <input type=“text” id=“nome” name=“nome”><br>
        <label for=“sobrenome”>Sobrenome:</label><br>
        <input type=“text” id=“sobrenome” name=“sobrenome”>
</form>
```
Podemos também usar o elemento <fieldset> para agrupar campos do formulário, como no exemplo a seguir:

```HTML
<form action=“/action_page.php”>
        <fieldset>
                <legend>Pessoa:</legend>
                <label for=“nome”>Nome:</label><br>
                <input type=“text” id=“nome” name=“nome” value=“John”><br>
                <label for=“sobrenome”>Sobrenome:</label><br>
                <input type=“text” id=“sobrenome” name=“sobrenome” value=“Doe”><br>
                <input type=“submit” value=“Submit”>
        </fieldset>
</form>

```
Podemos utilizar o atributo readonly para especificar que um campo de entrada é somente leitura. Um campo de entrada somente leitura não pode ser modificado.

Podemos usar também atributo maxlength para limitar número máximo de caracteres que podem ser inseridos em um campo.

A seguir mais um exemplo:

```HTML
<form>
        <label for=“nome”>Nome:</label>
        <input type=“text” id=“nome” name=“nome” value=“John” readonly>
        <label for=“sobrenome”>Sobrenome:</label>
        <input type=“text” id=“sobrenome” name=“sobrenome” value=“Doe” maxlength>
</form>
</form>
```
