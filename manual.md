# Manual do Repositório

## 1. Finalidade

Este repositório reúne atividades e trabalhos da disciplina em pastas separadas.

Na raiz, o acesso principal publicado pelo GitHub Pages redireciona automaticamente para `Atividade-2/index.html`.

## 2. Estrutura principal

- `Atividade-1/`: atividade 1.
- `Atividade-2/`: atividade 2 publicada como entrada principal do Pages.
- `Atividade-3/`: atividade 3.
- `Atividade-4/`: atividade 4.
- `Trabalho-1/`: trabalho 1.
- `index.html`: página raiz com redirecionamento imediato para `Atividade-2/index.html`.
- `.github/workflows/pages.yml`: workflow de deploy do GitHub Pages.
- `README.md`: descrição breve do repositório.

## 3. Regra de publicação

- o GitHub Pages publica a raiz do repositório;
- o arquivo `index.html` da raiz redireciona para `./Atividade-2/index.html`;
- o workflow `.github/workflows/pages.yml` executa o deploy da branch `main`;
- o artefato publicado corresponde ao conteúdo da raiz do repositório.

## 4. Regra de manutenção

- mudanças na atividade principal publicada devem preservar ou revisar conscientemente o redirecionamento da raiz;
- mudanças no fluxo de publicação devem ser refletidas neste `manual.md`;
- arquivos textuais do repositório devem permanecer em UTF-8 sem BOM.
