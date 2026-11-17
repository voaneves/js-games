# js-games

> **EN:** Classic browser games written in vanilla JavaScript: Tic-Tac-Toe, Rock-Paper-Scissors, Snake and Minesweeper. Static PWA, no frameworks or build step.

Coleção de jogos clássicos no navegador, escritos em JavaScript puro, sem frameworks e sem etapa de build.

**Jogue agora:** https://voaneves.github.io/js-games/

## Jogos

| Jogo | Código |
| :--- | :--- |
| Jogo da velha | `assets/js/tic-tac-toe.js` |
| Pedra, papel e tesoura | `assets/js/rock-paper-scissors.js` |
| Jogo da cobrinha (Snake), com botões direcionais na tela | `assets/js/snake.js` |
| Campo minado | `assets/js/mine.js` |

Também há tema claro e escuro (`prefers-color-scheme`), suporte a `prefers-reduced-motion` e instalação como PWA (`manifest.json` e `sw.js`).

## Rodar localmente

Não há dependências. Sirva a pasta com qualquer servidor estático (o service worker exige `http://localhost` ou HTTPS):

```bash
git clone https://github.com/voaneves/js-games.git
cd js-games
python -m http.server 8000
# abra http://localhost:8000
```

## Estrutura

```
index.html          página única com os jogos
manifest.json       manifesto do PWA
sw.js, worker.js    service workers (versões .min.js usadas na página)
assets/
  fonts/            fonte de ícones
  img/              ícones e imagens
  js/               um arquivo por jogo, mais app.js, cursor.js, console.js
  styles/           SCSS e CSS compilado (games.scss)
```

## Tecnologias

HTML, CSS/SCSS, JavaScript puro, Canvas (Snake), PWA.

## Licença

[MIT](LICENSE) © Victor Neves
