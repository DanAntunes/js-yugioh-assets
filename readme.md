# Yu-Gi-Oh Jo-Ke-Po Edition Web Game

Este projeto é um web game baseado no universo Yu-Gi-Oh, implementando uma versão do clássico jogo de Pedra, Papel e Tesoura com cartas e temática personalizada. Ele utiliza HTML, CSS e JavaScript para criar uma experiência interativa.

---

## Funcionalidades

1. **Temática Yu-Gi-Oh:**
   - Utiliza imagens, sons e vídeos inspirados no universo Yu-Gi-Oh para imersão.

2. **Dinâmica de Jogo:**
   - Escolha entre três cartas: Blue Eyes White Dragon, Dark Magician e Exodia, cada uma representando Pedra, Papel ou Tesoura.
   - Oponente (computador) escolhe aleatoriamente uma carta.

3. **Placar Dinâmico:**
   - Exibe vitórias e derrotas em tempo real.

4. **Interatividade:**
   - Mouseover para visualizar detalhes das cartas.
   - Feedback visual e sonoro para cada rodada.

5. **Execução Contínua:**
   - Permite reiniciar o duelo após cada rodada.

---

## Estrutura do Projeto

### **HTML**

- Estrutura principal da interface, incluindo:
  - Contêineres para cartas do jogador e do computador.
  - Área para exibição do placar.
  - Botão para reiniciar duelos.

### **CSS**

- Estilização personalizada com foco na temática Yu-Gi-Oh.
  - Arquivos adicionais para reset de estilos, botões e contêineres.
  - Uso da fonte `Press Start 2P` para remeter ao estilo retrô.
  - **buttons.css:** Define estilos detalhados para botões com diferentes estados (hover, active, etc.), incluindo variantes douradas e personalizadas.
  - **containers_and_frames.css:** Configurações de contêineres e quadros decorativos para áreas do jogo, como bordas temáticas e fundos personalizados.
  - **main.css:** Configurações principais do layout, incluindo cursores personalizados, vídeos de fundo e alinhamento responsivo dos elementos.
  - **reset.css:** Reinicializa estilos padrão para garantir consistência visual.

### **JavaScript**

- Lógica do jogo:
  - **Objetos principais:**
    - `state`: Gerencia o estado do jogo, como placar e cartas em jogo.
    - `cardData`: Define as cartas disponíveis, seus atributos e resultados possíveis contra outras cartas.
  - **Funções:**
    - `getRandomCardId()`: Seleciona uma carta aleatória para o computador.
    - `createCardImage()`: Cria elementos visuais para as cartas.
    - `setCardsField()`: Configura o campo de jogo com as cartas selecionadas.
    - `checkDuelResults()`: Verifica o vencedor de cada rodada.
    - `updateScore()`: Atualiza o placar.
    - `resetDuel()`: Reinicia o duelo.
  - **Áudio:** Sons de vitória e derrota para maior imersão.

---

## Como Jogar

1. **Início do Jogo:**
   - O jogo começa automaticamente com 5 cartas distribuídas para cada lado.
   - O áudio de fundo será reproduzido automaticamente (certifique-se de ativar o som no navegador).

2. **Seleção de Cartas:**
   - Passe o mouse sobre as cartas disponíveis para visualizar seus detalhes.
   - Clique em uma carta para escolher sua jogada.

3. **Resultado do Duelo:**
   - Após escolher sua carta, o computador também revelará a sua.
   - O resultado (vitória, derrota ou empate) será exibido.

4. **Reinício:**
   - Clique no botão "GANHOU" ou equivalente para começar uma nova rodada.

---

## Tecnologias Utilizadas

- **HTML5**: Estrutura da página.
- **CSS3**: Estilização visual.
- **JavaScript (ES6+)**: Lógica e interatividade do jogo.

---

## Estrutura de Arquivos

```plaintext
src/
├── assets/
│   ├── audios/
│   │   ├── egyptian_duel.mp3
│   │   ├── win.wav
│   │   └── lose.wav
│   ├── favicon/
│   │   └── Favicon.ico
│   ├── icons/
│   │   ├── card-back.png
│   │   ├── dragon.png
│   │   ├── magician.png
│   │   └── exodia.png
│   └── video/
│       └── yugi.mp4
├── scripts/
│   └── engine.js
├── styles/
│   ├── reset.css
│   ├── buttons.css
│   ├── containers_and_frames.css
│   └── main.css
└── index.html
```

---

## Como Executar

1. Clone este repositório:

   ```bash
   git clone <URL_DO_REPOSITORIO>
   ```

2. Navegue até o diretório do projeto:

   ```bash
   cd yu-gi-oh-joke-po
   ```

3. Abra o arquivo `index.html` no navegador de sua preferência.

---

## Melhorias Futuras

- Adicionar níveis de dificuldade.
- Implementar modo multiplayer.
- Expandir o conjunto de cartas disponíveis.
- Melhorar a responsividade para dispositivos móveis.

---

## Autor

Este projeto foi desenvolvido como um exemplo prático para aprimorar habilidades em desenvolvimento web e criar uma experiência divertida e interativa. Caso tenha dúvidas ou sugestões, sinta-se à vontade para contribuir!

