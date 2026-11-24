# A Fraude da Enron e a Falha da Auditoria Contábil

Apresentação web em 3D do trabalho acadêmico de Ciências Contábeis
**"A fraude da Enron e a falha da auditoria contábil: impactos e aprendizados para a profissão"**.

Cada seção do trabalho é uma sala em um andar do prédio da Enron. A câmera entra no prédio
e sobe de andar em andar, e as telas de cada sala mostram mapas, linhas do tempo e gráficos com dados reais.

![Capa](imagens/capa.jpg)

## ▶️ Ver a apresentação

**Online:** `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/` *(depois de ativar o GitHub Pages; veja abaixo)*

**No computador, sem internet:** baixe [`download/Apresentacao-Enron.zip`](download/Apresentacao-Enron.zip),
extraia e dê dois cliques em `APRESENTAR (Windows).bat`. No Mac, use `Apresentar (Mac).command`.
A apresentação abre em tela cheia, como um aplicativo.

| Sala do térreo | Sala da fraude (andar 24) | Sala da empresa (andar 12) |
|---|---|---|
| ![](imagens/sala-lobby.jpg) | ![](imagens/sala-fraude.jpg) | ![](imagens/sala-mapa.jpg) |

## Roteiro (slides)

| Slide | Seção do trabalho | Sala |
|---|---|---|
| 1 | Capa | Vista externa do prédio |
| 2 | Resumo e Introdução | Lobby |
| 3 | A Enron e sua ascensão | Escritório executivo: mapa e linha do tempo |
| 4 | A fraude: MTM, SPVs e manipulação | Sala de reunião com gráficos |
| 5 | A auditoria e a Arthur Andersen | Arthur Andersen |
| 6 | A investigação | Força-tarefa |
| 7 | Impactos e a Lei Sarbanes-Oxley | Mesa de operações |
| 8 | Aprendizados para a profissão | Sala do conselho |
| 9 | Considerações finais e Referências | Vista aérea do topo |

## ⌨️ Controles

| Tecla / ação | Função |
|---|---|
| → · espaço · PageDown · roda do mouse | Avançar (passadores de slide funcionam) |
| ← · PageUp | Voltar |
| **F** ou botão ⛶ | Tela cheia |
| **Z** · duplo clique · botão ⤢ | Ampliar a tela da sala em 2D (Esc fecha) |
| Home / End | Capa / conclusão |
| Menu do topo ou elevador à direita | Ir direto para uma seção |

Link direto para uma seção: `index.html#fraude`, `#auditoria`, `#impactos` etc.

## 🌐 Publicar no GitHub Pages

1. No repositório, abra **Settings → Pages**.
2. Em **Build and deployment → Source**, escolha **Deploy from a branch**.
3. Selecione o branch **main** e a pasta **/ (root)**. Depois clique em **Save**.
4. Em 1 ou 2 minutos o endereço aparece no topo da página. Coloque esse endereço no lugar do link "Online" acima.

O site também é um app instalável (PWA): no Chrome ou Edge aparece o botão **Instalar** na barra de endereço.

## 🛠️ Editar

O site publicado (`index.html`, `predio-3d.html`) é **gerado** a partir de `codigo-fonte/`:

| Arquivo | Conteúdo |
|---|---|
| `codigo-fonte/src/content.js` | Textos do painel lateral de cada seção |
| `codigo-fonte/src/screens.js` | Telas e gráficos dentro das salas |
| `codigo-fonte/src/rooms.js` | Salas, móveis e posição da câmera |
| `codigo-fonte/src/world.js` | Prédio, cidade, céu e reflexos |
| `codigo-fonte/src/app.js` | Navegação, transições, tela cheia |
| `codigo-fonte/capa.html` | Capa, menu, painel e estilos |

Depois de editar, gere o site de novo. É preciso ter o [Node.js](https://nodejs.org) instalado:

```bash
cd codigo-fonte
npm install      # só na primeira vez
npm run build    # atualiza index.html e predio-3d.html na raiz
```

Feito com [three.js](https://threejs.org) e empacotado com [esbuild](https://esbuild.github.io).
O resultado é um arquivo HTML único que funciona sem internet.

## Fontes dos dados

- Encyclopaedia Britannica: *Enron scandal*
- FBI: *Enron* (Famous Cases & Criminals)
- Investopedia: *Enron Scandal: The Fall of a Wall Street Darling*
- Sarbanes-Oxley Act of 2002 (Public Law 107-204)
- Enron Corp., *Annual Report 2000*: receitas e lucros de 1996 a 2000

---

Trabalho acadêmico com fins educacionais. "Enron" e o logotipo pertencem aos seus respectivos titulares.
O prédio 3D é uma recriação artística.
