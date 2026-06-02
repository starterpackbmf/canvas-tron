# Canvas Tron

Editor de mapa mental com estética Tron/Jarvis — blocos editáveis, conexões ortogonais com gradiente, anotações ricas e desenho livre.

## Features

- **Blocos** editáveis com título + corpo (negrito, itálico, sublinhado, tamanho, cor)
- **Conexões ortogonais** com cantos arredondados e gradiente da cor da origem até a cor do destino
- **Recolher/expandir** ramos clicando nas portas
- **Apagar conexão** (clica na linha, Del)
- **Criar bloco conectado** arrastando de uma porta pro vazio
- **Ferramenta unificada de anotação**: texto, pincel livre, linha, seta, retângulo, elipse, borracha
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
