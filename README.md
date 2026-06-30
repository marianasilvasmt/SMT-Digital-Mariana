# Área de Testes — Surveys

Página interna para testar surveys antes de irem ao ar, protegida por senha.

## Estrutura

- `index.html` — tela de login. Pede uma senha antes de liberar o acesso.
- `home.html` — dashboard com os cards de cada survey disponível para teste.
- `survey-teste.html` — modelo de página de teste. Duplique este arquivo para cada nova survey, renomeie e troque o link/embed.

## Como configurar a senha

1. Abra `gerar-hash.html` (não versionado/local) no navegador.
2. Digite a senha desejada e copie o hash gerado.
3. Cole o hash em `index.html`, na linha que contém `targetHash`.

## Como adicionar uma nova survey

1. Duplique `survey-teste.html` e renomeie (ex: `795-tests.html`).
2. Edite o link/embed da survey dentro do arquivo.
3. No `home.html`, adicione um novo card no `tools-grid` apontando para esse arquivo.

## Deploy

O site é estático (HTML/CSS/JS puro). Pode ser publicado via:
- **Vercel** — importar o repositório em vercel.com.
- **GitHub Pages** — Settings → Pages → Source: branch `main`, pasta `/root`.