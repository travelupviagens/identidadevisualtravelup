# Travel Up — Identidade Visual

Repositório canônico da identidade visual da **Travel Up**, agência de viagens especializada em emissão de passagens com milhas, fundada por Paula Fortini.

## Para que serve este repositório

Este repositório é escrito para ser lido por modelos de linguagem (LLMs), não por humanos. Qualquer agente que precise produzir material da marca (post, apresentação, orçamento, landing page, card de WhatsApp, e-mail) deve ler os arquivos daqui antes de escolher cor, fonte, tom de voz ou versão de logo.

Princípios de organização:

- Markdown puro, sem HTML.
- Hierarquia rasa. No máximo três níveis.
- Cada `.md` é autocontido: dá para responder uma pergunta lendo só um arquivo.
- Texto no lugar de imagem sempre que possível. Cores são hex escritos, não amostras. Variações de logo são descritas em tabela, não só mostradas.

## Índice

| Arquivo | O que responde |
|---|---|
| `marca/manifesto-e-posicionamento.md` | O que a marca é, para quem fala, como fala |
| `marca/briefing-original.md` | Briefing que originou a identidade, transcrito |
| `identidade-visual/cores.md` | Paleta com hex exatos, contraste e regras de uso |
| `identidade-visual/tipografia.md` | Fontes, pesos, eixos variáveis, CSS pronto |
| `identidade-visual/logotipo-e-submarca.md` | Inventário das 19 variações de logo e submarca, com regra de qual usar |

## Resumo executivo

Para um agente que só precisa do essencial:

- **Marca:** Travel Up. Escrita `Travel Up` em texto corrido. O logotipo grafa `travel up` em caixa baixa.
- **Fundadora:** Paula Fortini.
- **O que faz:** acesso a passagens mais baratas via uso estratégico de milhas, sem complicação e com transparência.
- **Público:** pessoas de médio e alto padrão que querem economizar em passagem sem perder tempo com informação técnica ou confusa.
- **Tom de voz:** direto ao ponto, empático, amigável, inteligente, descomplicado. Sem jargão de milhas sem explicação.
- **Cor principal:** azul principal `#24356D`.
- **Cor de destaque:** azul claro `#A5D9EC`.
- **Fonte de título:** Bricolage Grotesque.
- **Fonte de texto:** Montserrat.
- **Estética:** minimalista, elegante, neutra. Nada de cor forte ou quente, que puxa a leitura para varejo.

## Estrutura de pastas

```
travel-up-brand/
├── README.md
├── marca/
│   ├── manifesto-e-posicionamento.md
│   └── briefing-original.md
├── identidade-visual/
│   ├── logotipo-e-submarca.md
│   ├── cores.md
│   └── tipografia.md
└── assets/
    ├── logos/
    │   ├── svg/    19 arquivos vetoriais, fonte da verdade
    │   └── png/    os mesmos 19, 1600x900px
    ├── fontes/
    │   ├── bricolage-grotesque/
    │   └── montserrat/
    └── editaveis/
        └── travel-up-arquivo-editavel.ai
```

## Nomenclatura dos arquivos de asset

Todo asset segue o padrão `{tipo}-{cor-da-marca}-fundo-{cor-do-fundo}.{ext}`, em minúsculas, sem acento e sem espaço.

Exemplos:

- `logo-azul-principal-fundo-transparente.svg` — logotipo completo em `#24356D`, fundo transparente.
- `submarca-branca-fundo-azul-principal.png` — submarca em branco sobre fundo `#24356D`.

Os nomes originais entregues pelo estúdio tinham espaços, acentos e três erros de rotulagem. Foram renomeados. O mapeamento completo entre nome original e nome novo está em `identidade-visual/logotipo-e-submarca.md`.

## Grau de confiabilidade das informações

Este repositório distingue o que foi verificado do que foi inferido. Cada arquivo marca isso explicitamente onde há dúvida.

- **Cores:** verificadas. Os hex foram lidos direto do código dos arquivos SVG, que são exportação vetorial do arquivo original do estúdio. São valores de especificação, não amostragem.
- **Fontes:** verificadas. Nome, versão, licença e eixos variáveis lidos das tabelas internas dos arquivos `.ttf`.
- **Inventário de logos:** verificado. Cada variação foi conferida pelo hex declarado dentro do SVG.
- **Manifesto e posicionamento:** transcrição do manual de identidade em PDF.
- **Briefing:** transcrição do PDF `Shark Briefing - Travel UP.pdf`.

## O que não está neste repositório

- `TRAVEL UP - MANUAL DE IDENTIDADE.pdf` (13 páginas, ~52MB) e sua versão em `.pptx` (~111MB). Ficaram fora por tamanho. O conteúdo textual relevante foi extraído para os `.md` deste repositório.
- `First View - Travel Up.psd` (~174MB). Excede o limite de 100MB por arquivo do GitHub.
- `Travel Up - Arquivo Editável.eps` (~8,9MB). Redundante com o `.ai`, que está incluído.
- Pesos estáticos das fontes (126 arquivos `.ttf`). Só as fontes variáveis estão versionadas aqui. Os estáticos são recuperáveis no Google Fonts.

Os originais completos ficam no Google Drive da Travel Up, na pasta de identidade visual.
