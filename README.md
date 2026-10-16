# Air Hockey Game

Jogo arcade de air hockey para uma pessoa contra a CPU. Mova o rebatedor para defender seu lado e devolver o disco; vence quem marcar **7 gols primeiro**.

## Como jogar

- Mova o mouse sobre a arena para controlar o rebatedor azul. Em telas sensíveis ao toque, arraste o dedo sobre a mesa.
- O rebatedor do jogador fica limitado à metade esquerda da mesa.
- Pressione **S** para alternar o som. O jogo começa com o áudio silenciado.
- A partida inicia automaticamente ao abrir a página. Depois do resultado, use **PLAY AGAIN** ou pressione **Espaço** para jogar novamente.

## Recursos

- Partida contra um oponente controlado por IA.
- Física de disco com atrito, rebotes nas bordas e colisões com os rebatedores.
- Pontuação até 7, sequências de gols, velocidade máxima do disco e contagem de rebatidas fortes.
- A velocidade aumenta progressivamente durante a partida; momentos de game point recebem efeito de câmera lenta.
- Efeitos visuais de neon, partículas, vibração de tela e confete na vitória.
- Efeitos sonoros sintetizados com a Web Audio API.

## Executar localmente

Não é necessário instalar dependências ou compilar o projeto. Para servir os arquivos localmente, execute na pasta do projeto:

```bash
python3 -m http.server 8000
```

Abra <http://localhost:8000> em um navegador moderno. A interface está em inglês. O jogo usa o elemento Canvas 2D; fontes e estilos externos são carregados por CDN, então a conexão com a internet é necessária para esses recursos externos.

## Tecnologias e arquivos

- HTML, CSS e JavaScript sem processo de build.
- Canvas 2D e Web Audio API do navegador.
- `index.html` — interface, arena e referências às fontes/estilos externos.
- `style.css` — layout, painel de pontuação e efeitos visuais.
- `script.js` — física, IA da CPU, controles, pontuação, renderização e áudio.
