Essa é uma excelente ideia para um projeto\! Uma **página pessoal** (ou portfólio simples) é um projeto clássico que permite praticar HTML e CSS de forma integrada, e 3 horas é um bom prazo para desenvolver a estrutura e o estilo básico.

Aqui está o projeto detalhado, com foco nas habilidades a serem praticadas e um cronograma sugerido.

-----

## Projeto: Página Pessoal Simples

### Objetivo

Construir uma **página pessoal estática** utilizando apenas **HTML e CSS** para exibir informações básicas sobre você, suas habilidades e um meio de contato.

### Estrutura do Projeto

Crie uma pasta principal para o projeto e dentro dela, crie os seguintes arquivos:

1.  `index.html` (para o conteúdo e estrutura)
2.  `styles.css` (para a estilização)

### Cronograma Sugerido (Aproximado)

| Fase | Duração Sugerida | Foco Principal |
| :--- | :--- | :--- |
| **Fase 1:** Estrutura HTML | 60 minutos | Semântica, Conteúdo, Links. |
| **Fase 2:** Estilização Básica (Reset & Layout) | 60 minutos | CSS Reset, Fontes, Cores, **Flexbox**. |
| **Fase 3:** Estilização Detalhada & Responsividade | 60 minutos | Estilos específicos, Coerência Visual, **Media Queries**. |
| **Total** | **3 horas** | |

-----

## Fase 1: Estrutura HTML (`index.html`)

O foco aqui é na **semântica** e organização do conteúdo. Não se preocupe com a aparência por enquanto.

### Elementos Chave a Incluir

1.  **Cabeçalho (`<header>`):**

      * Seu nome/título principal (`<h1>`).
      * Uma breve navegação (`<nav>` com lista `<ul>`) contendo links âncora (ex: `#sobre`, `#habilidades`, `#contato`).

2.  **Seção "Sobre Mim" (`<section>` com `id="sobre"`):**

      * Um título secundário (`<h2>`).
      * Um parágrafo (`<p>`) de introdução sobre quem você é.
      * Opcional: Uma imagem sua (`<img>`).

3.  **Seção "Habilidades" (`<section>` com `id="habilidades"`):**

      * Um título secundário (`<h2>`).
      * Uma lista de habilidades (`<ul>` ou `<dl>`) em tópicos (ex: HTML, CSS, JavaScript, Inglês, etc.).

4.  **Seção "Contato" (`<section>` com `id="contato"`):**

      * Um título secundário (`<h2>`).
      * Links para suas redes sociais ou email (utilize o elemento âncora `<a>`).
      * Opcional: Um formulário de contato simples (`<form>`) (apenas a estrutura, sem funcionalidade no *backend*).

5.  **Rodapé (`<footer>`):**

      * Informações de *copyright* e ano atual (`<p>`).

-----

## Fase 2: Estilização Básica e Layout (`styles.css`)

Conecte seu `styles.css` ao `index.html` (dentro do `<head>`) e comece a dar forma à página.

### Estilização Essencial a Aplicar

1.  **CSS Reset:**

      * Defina `margin: 0;` e `padding: 0;` para todos os elementos ou os mais comuns (body, ul, h1-h6, p).
      * Use `box-sizing: border-box;` globalmente (`*`).

2.  **Tipografia:**

      * Defina uma **fonte principal** para o `<body>` (pode ser uma fonte do Google Fonts).
      * Defina **tamanhos de fonte** base e específicos para `<h1>`, `<h2>`, e parágrafos.

3.  **Cores:**

      * Escolha uma paleta de cores simples (uma principal, uma de fundo e uma de destaque).

4.  **Layout com Flexbox (***Habilidade Principal***):**

      * Use **Flexbox** para:
          * **Centralizar** os itens da navegação (`<nav>`).
          * Organizar as habilidades em **linhas ou colunas** (como "cards" lado a lado).
          * Distribuir o conteúdo principal dentro da página.

5.  **Estilização do Cabeçalho e Navegação:**

      * Dê ao `<header>` uma cor de fundo e fixe-o no topo da tela (`position: fixed;` ou `position: sticky;` - *desafio*).
      * Remova os marcadores de lista dos itens de navegação (`list-style: none;`).

-----

## Fase 3: Estilização Detalhada e Responsividade

Agora, refine a aparência e certifique-se de que a página funcione bem em diferentes dispositivos.

### Detalhes de Estilo

1.  **Design de Componentes:**

      * Estilize os "cards" de habilidades (adicionar bordas, `padding`, `box-shadow`).
      * Estilize os *links* para que mudem de cor ou ganhem um sublinhado ao passar o *mouse* (`:hover`).

2.  **Espaçamento:**

      * Adicione margens e preenchimentos (`margin` e `padding`) consistentes para criar "espaço em branco" e melhorar a legibilidade entre as seções.

### Responsividade (***Habilidade Principal***)

1.  **Media Query:**
      * Crie uma **media query** para telas menores (ex: `max-width: 768px`).
      * Dentro dela, **ajuste o layout do Flexbox** para que os itens que estavam lado a lado (como a navegação ou as habilidades) passem a se empilhar verticalmente.
      * Reduza o tamanho da fonte ou dos *paddings* para dispositivos móveis, se necessário.

<!-- end list -->

```css
/* Exemplo de Media Query */
@media (max-width: 768px) {
    /* Mude a direção do Flexbox na navegação */
    nav ul {
        flex-direction: column;
        align-items: center;
    }

    /* Faça as habilidades ocuparem a largura total */
    .habilidade-card {
        width: 90%;
        margin-bottom: 20px;
    }
}
```

-----

## Check-list Rápido

Ao final das 3 horas, verifique se você conseguiu:

| Recurso/Habilidade | Concluído? |
| :--- | :--- |
| Estrutura básica HTML com semântica correta (`<header>`, `<nav>`, `<section>`, `<footer>`). | $\square$ |
| Links âncora funcionando para navegar entre as seções. | $\square$ |
| Uso de **Flexbox** para organizar pelo menos um bloco da página (ex: navegação ou habilidades). | $\square$ |
| Estilização de cores e tipografia consistente. | $\square$ |
| Uso de **pseudoclasses** (`:hover` em links ou botões). | $\square$ |
| Uso de **Media Queries** para ajustar o layout em telas menores. | $\square$ |

-----

Ao concluir, você terá um bom ponto de partida para um portfólio e terá praticado as habilidades fundamentais de HTML e CSS\! O que achou do projeto?