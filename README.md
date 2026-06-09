# IA, linguagem e responsabilidade humana

Landing page estática da obra em quatro livros de **Ibrahim J. Jamhour**.

Site editorial, sem frameworks nem backend. Publicado em [ijamhour.github.io/obra-ia](https://ijamhour.github.io/obra-ia/).

A **v2** inclui orientação por interesses de leitura, trechos de degustação e links UICLAP como canal principal da obra em português.

## Estrutura

```
obra-ia/
├── index.html
├── styles.css
├── assets/
└── README.md
```

## Imagens

Capas em `assets/`:

| Arquivo | Livro |
|---------|-------|
| `experimento.jpg` | O Experimento que Somos |
| `pensar-falar.jpg` | Entre o Pensar e o Falar |
| `crise-competencia.jpg` | A Crise da Competência |
| `resposta-pronta.jpg` | Depois da Resposta Pronta |

Opcionais: `social-card.jpg` (Open Graph), `favicon.ico`.

## Links UICLAP

| Livro | URL |
|-------|-----|
| O Experimento que Somos | https://loja.uiclap.com/titulo/ua163865 |
| Entre o Pensar e o Falar | https://loja.uiclap.com/titulo/ua174970 |
| A Crise da Competência | https://loja.uiclap.com/titulo/ua177225 |
| Depois da Resposta Pronta | https://loja.uiclap.com/titulo/ua175880 |

Links Amazon e versões internacionais poderão ser adicionados futuramente, quando houver edições em português ou em seção separada.

## Testar localmente

```bash
python -m http.server 8000
# ou: npx serve .
```

## Publicar via GitHub Pages

Settings → Pages → branch `main`, pasta `/ (root)`.

Metadados Open Graph em `index.html` apontam para `https://ijamhour.github.io/obra-ia/`.
