# IA, linguagem e responsabilidade humana

Landing page estática da obra em quatro livros de **Ibrahim J. Jamhour**.

Site editorial, sem frameworks nem backend. Preparado para [GitHub Pages](https://pages.github.com/).

## Estrutura

```
obra-ia/
├── index.html      # Conteúdo e metadados
├── styles.css      # Estilos
├── assets/         # Imagens
└── README.md
```

## 1. Substituir imagens

Coloque as capas na pasta `assets/`:

| Arquivo | Livro |
|---------|-------|
| `experimento.jpg` | O Experimento que Somos |
| `pensar-falar.jpg` | Entre o Pensar e o Falar |
| `crise-competencia.jpg` | A Crise da Competência |
| `resposta-pronta.jpg` | Depois da Resposta Pronta |

Opcionais — a página funciona normalmente se ainda não existirem:

| Arquivo | Uso |
|---------|-----|
| `author.jpg` | Foto do autor (some discretamente se ausente) |
| `social-card.jpg` | Imagem para compartilhamento (Open Graph) |
| `favicon.ico` | Ícone do navegador |

Proporção recomendada das capas: **2:3** (retrato). Se uma capa não carregar, o título do livro aparece como placeholder no espaço da imagem.

## 2. Links de compra (UICLAP)

A primeira versão da página usa **apenas links UICLAP** para os livros em português. Os endereços ativos estão nos cards de `index.html` e documentados no bloco **METADADOS EDITÁVEIS** no topo do arquivo:

| Livro | UICLAP |
|-------|--------|
| O Experimento que Somos | `https://loja.uiclap.com/titulo/ua163865` |
| Entre o Pensar e o Falar | `https://loja.uiclap.com/titulo/ua174970` |
| A Crise da Competência | `https://loja.uiclap.com/titulo/ua177225` |
| Depois da Resposta Pronta | `https://loja.uiclap.com/titulo/ua175880` |

Para alterar um link, edite o `href` do botão correspondente no card do livro.

A chamada final da página direciona para a seção de livros (`#livros`).

### Amazon e versões internacionais

Links Amazon **não aparecem** nesta primeira versão — ainda não há edições em português na Amazon.

Quando existirem edições em português, os botões Amazon poderão ser adicionados de volta aos cards. Os placeholders estão marcados como *a incluir futuramente* no bloco de metadados.

Versões internacionais do primeiro livro (inglês e espanhol) podem ser tratadas depois em uma seção separada, se desejado, sem substituir os botões principais da obra em português.

Depois de publicar, substitua `SEU-USUARIO` nos metadados Open Graph (`og:url` e `og:image`) pelo endereço real do GitHub Pages.

## 3. Testar localmente

Abra `index.html` no navegador, ou use um servidor local:

```bash
# Python 3
python -m http.server 8000

# Node.js (npx, sem instalar)
npx serve .
```

Acesse `http://localhost:8000`.

## 4. Publicar via GitHub Pages

1. Crie um repositório no GitHub (ex.: `obra-ia`).
2. Envie os arquivos para a branch `main`.
3. No repositório: **Settings → Pages**.
4. Em **Source**, escolha **Deploy from a branch**.
5. Selecione branch `main` e pasta **`/ (root)`**.
6. Salve. Em alguns minutos o site estará em `https://SEU-USUARIO.github.io/obra-ia/`.

## Metadados SEO

Edite no `<head>` de `index.html`, se necessário:

- `<title>`
- `<meta name="description">`
- `<meta property="og:title">`
- `<meta property="og:description">`
- `<meta property="og:image">`

Referência completa no bloco de comentários no início do arquivo.
