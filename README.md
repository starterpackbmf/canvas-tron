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
- **Salvar/Carregar** em JSON
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
- `Del` Apagar seleção
- `Esc` Cancelar / sair de edição
- Duplo clique vazio → novo bloco
