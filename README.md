# Canvas Tron

Editor de mapa mental com estética Tron/Jarvis — blocos editáveis, conexões ortogonais com gradiente, anotações ricas e desenho livre.

## Features

- **Blocos** editáveis com título + corpo (negrito, itálico, sublinhado, tamanho, cor)
- **Conexões editáveis e livres**: arraste a linha pra criar uma dobra (waypoint), arraste a dobra pra moldar, duplo-clique remove; clique na conexão pra ver as alças e um botão que alterna o **estilo** (ortogonal / curva suave / reta); arraste as **pontas** pra reconectar em outra porta sem refazer
- **Conexões** com gradiente da cor da origem até a cor do destino e fluxo de energia animado seguindo o caminho
- **Recolher/expandir** ramos clicando nas portas
- **Apagar conexão** (clica na linha, Del)
- **Criar bloco conectado** arrastando de uma porta pro vazio
- **Anotação (texto)** e **Desenho** (pincel livre, linha, seta, retângulo, elipse, borracha) em ferramentas separadas
- **Moldura da anotação** opcional — toggle pra deixar só o texto, sem a caixa em volta
- **Preenchimento** de retângulo e elipse — liga/desliga, com cor e opacidade ajustáveis (slider); editável também depois de desenhado
- **Redimensionar blocos** pelas 4 alças de canto
- **Paleta de cores** contextual por tipo de elemento (bloco, traço, texto)
- **Desfazer/Refazer** (`Ctrl+Z` / `Ctrl+Shift+Z` ou `Ctrl+Y`) — histórico de até 120 passos
- **Autosave** — o trabalho é salvo automaticamente no navegador (localStorage) e restaurado ao reabrir
- **Duplicar seleção** (`Ctrl+D`) — copia blocos, anotações, traços e as conexões internas
- **Modo apresentação** (`P` ou botão `▶ APRESENTAR`) — destaca um bloco por vez, escurece o resto e dá zoom suave; navega com `←` `→` (ou espaço)
- **Fluxo de energia** — pulso animado correndo pelas conexões, no estilo Tron (botão `⚡ FLUXO` liga/desliga)
- **Salvar/Carregar** em JSON
- **Exportar PNG** — gera uma imagem do mapa inteiro pra compartilhar
- **Pan** (arrastar canvas) e **zoom** (roda do mouse)

## Stack

- React 18 via CDN (UMD)
- Babel Standalone (transpile JSX no browser)
- SVG para linhas, paths, e gradientes
- Arquivo único `index.html` — sem build step

## Como rodar localmente

Abre `index.html` direto no navegador, ou sobe um servidor:

```bash
python -m http.server 8765
# acessa http://localhost:8765
```

## Atalhos

- `V` Selecionar
- `B` Novo bloco
- `N` Texto (anotação)
- `D` Desenho livre
- `P` Modo apresentação
- `Ctrl+Z` / `Ctrl+Shift+Z` Desfazer / Refazer
- `Ctrl+D` Duplicar seleção
- `Del` Apagar seleção
- `Esc` Cancelar / sair de edição / sair da apresentação
- Duplo clique vazio → novo bloco
- No modo apresentação: `←` `→` (ou espaço) navega entre os blocos
