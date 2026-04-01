# Mars Books

Repositorio de dados dos livros do **Projeto Marte**.

## Estrutura

```
index.json                    ← Lista de IDs dos livros publicados
astounding-1930-12/
  book.json                   ← Metadados do livro
  cover.jpg                   ← Capa do livro
  before-01.jpg               ← Imagem original 1
  after-01.jpg                ← Imagem remasterizada 1
  before-02.jpg               ← Imagem original 2
  after-02.jpg                ← Imagem remasterizada 2
```

## Como adicionar um novo livro

1. Crie uma pasta com o ID do livro (ex: `astounding-1931-07`)
2. Adicione o `book.json` com os metadados (use outro como modelo)
3. Adicione `cover.jpg` com a capa do livro
4. Adicione pares de imagens `before-XX.jpg` / `after-XX.jpg`
5. Coloque os PDFs na pasta e atualize os campos `downloads.pdf` e `downloadsPt.pdf` no `book.json`
6. Adicione o ID no `index.json`
7. Commit e push

## Campos do book.json

| Campo | Descricao |
|-------|-----------|
| `downloads.pdf` | Link/caminho do PDF em ingles |
| `downloadsPt.pdf` | Link/caminho do PDF traduzido (PT) |
| `uiclapUrl` | Link para comprar fisico traduzido |
| `uiclapUrlEn` | Link para comprar fisico em ingles |
| `images` | Array de `{ before, after, caption }` |
| `status` | `published` ou `draft` |
