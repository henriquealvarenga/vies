# Viés e Erro em Pesquisa Epidemiológica

Material didático aberto sobre **erro sistemático, viés, fatores de
confusão em pesquisa epidemiológica** — para
alunos de Medicina e áreas afins.

Site construído em [Quarto](https://quarto.org), publicado via GitHub
Pages, licenciado sob MIT.

## Estrutura do repositório

```
Vies_Bias_Projetc/
├── _quarto.yml              # Configuração do site (navbar, sidebar, formatos)
├── index.qmd                # Landing page
├── creditos.qmd             # Créditos, autor, licença, como citar
├── referencias.qmd          # Página de bibliografia
├── theme-editorial.scss     # Tema visual SCSS (editorial, fundo claro)
├── styles.css               # CSS adicional (overrides finos)
│
├── conceitos/               # Conceitos fundamentais
│   ├── erro-sistematico-aleatorio.qmd
│   ├── definicao-vies.qmd
│   ├── vies-vs-confusao.qmd
│   ├── relacoes-espurias.qmd
│   └── variaveis-dependentes-independentes.qmd
│
├── tipos-vies/              # As quatro grandes famílias de viés
│   ├── vies-selecao.qmd
│   ├── vies-afericao.qmd
│   ├── vies-memoria.qmd
│   └── vies-nao-resposta.qmd
│
├── nominados/               # Vieses com nome próprio
│   ├── vies-berkson.qmd
│   ├── vies-neyman.qmd
│   ├── healthy-worker.qmd
│   ├── falacia-ecologica.qmd
│   ├── falacia-atomistica.qmd
│   ├── vies-perda-seguimento.qmd
│   ├── vies-afericao-diferencial.qmd
│   ├── vies-entrevistador.qmd
│   ├── vies-deteccao.qmd
│   ├── vies-publicacao.qmd
│   └── vies-lead-time.qmd
│
├── delineamentos/           # Vieses por delineamento de estudo
│   ├── transversais.qmd
│   ├── ecologicos.qmd
│   ├── coorte.qmd
│   └── caso-controle.qmd
│
├── casos/                   # Estudos de caso clássicos
│   ├── literary-digest-1936.qmd
│   ├── hite-report.qmd
│   └── alcool-mortalidade.qmd
│
├── slides/                  # Apresentação Reveal.js
│   └── tipos-de-vies.qmd
│
├── material-alunos/         # Atividade para discentes
│   └── instrucoes-trabalho.qmd
│
├── references/              # Bibliografia e estilos de citação
│   ├── referencias.bib      # BibTeX com referências canônicas
│   └── csl_styles/          # Estilos CSL (Vancouver, ABNT, APA, BJP)
│       ├── vancouver.csl    # ATIVO no _quarto.yml
│       ├── ABNT.csl
│       ├── apa.csl
│       └── ...
│
├── images/                  # Imagens (atualmente vazio)
└── data/                    # Conjuntos de dados auxiliares (atualmente vazio)
```

## Como compilar

Requisitos:

- [Quarto](https://quarto.org/docs/get-started/) (≥ 1.4)
- Opcional: R ou Python se chunks executáveis forem adicionados

Para gerar localmente:

```bash
# Compilar todo o site
quarto render

# Servidor de desenvolvimento com hot-reload
quarto preview
```

O site é gerado em `_site/`. A pasta está ignorada pelo `.gitignore`
— a publicação é feita por workflow.

## Publicação

A publicação recomendada é via **GitHub Pages**. Após o primeiro
`git push`:

1. No repositório, ir em **Settings → Pages**.
2. Em **Source**, escolher **GitHub Actions**.
3. Adicionar workflow `.github/workflows/publish.yml` com a action
   `quarto-dev/quarto-actions/publish@v2`.

## Citação

Para citar o material:

> Silva HA. Viés e Erro em Pesquisa Epidemiológica [Internet]. 2026.
> Disponível em: https://henriquealvarenga.github.io/vies/

Formato Vancouver. Outros formatos (ABNT, APA) estão na página de
[Créditos](creditos.qmd).

## Autor

**Prof. Henrique Alvarenga da Silva**
Médico psiquiatra · Mestre em Ensino em Saúde
Cursos de Medicina UFSJ e UNIPTAN

- 🌐 <https://www.henriquealvarenga.com>
- 🆔 ORCID: [0000-0001-9799-5240](https://orcid.org/0000-0001-9799-5240)
- 📚 [Currículo Lattes](http://lattes.cnpq.br/6147640440978297)

## Licença

[MIT](LICENSE) — uso em sala de aula, redistribuição e adaptação são
livres, desde que o aviso de copyright seja preservado.

## Contribuições

Issues e pull requests são bem-vindos — seja para correções de conteúdo
(erros factuais), sugestões de novos tópicos, melhorias de
acessibilidade ou tradução para outros idiomas.
