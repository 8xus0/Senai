O Genius Game é um jogo de memória onde o jogador deve seguir e repetir uma sequência de cores que é gerada aleatoriamente. A cada nível, a sequência de cores aumenta, tornando o jogo mais desafiador. O jogo conta com 3 níveis de dificuldade e oferece visual durante o jogo, como imagens e mensagens de erro/vitória.

Funcionalidades:
Geração de Sequência de Cores: O jogo gera uma sequência aleatória de cores, e o jogador deve reproduzi-la ao clicar nos botões correspondentes.

Três Níveis de Dificuldade:
- Fácil: 10 sequências e tempo de resposta mais longo.
- Médio: 25 sequências e tempo de resposta intermediário.
- Difícil: 50equências e tempo de resposta mais curto.

Visual: O jogo exibe imagens durante o jogo, mostrando diferentes estágios (erro, vitória, início).

Tela de Erro: Exibe uma tela de erro quando o jogador falha ao repetir a sequência corretamente.

Tela de Vitória: Exibe uma tela de vitória quando o jogador vence o jogo.

Tecnologias Utilizadas:
- React Native: Framework utilizado para desenvolvimento do aplicativo mobile.
- JavaScript (ES6): Utilizado para implementar a lógica de funcionamento do jogo.
- StyleSheet: Para estilizar os componentes da interface.

Como Jogar:
1. Escolha a Dificuldade: Ao iniciar o jogo, o jogador escolhe a dificuldade entre Fácil, Médio e Difícil.
2. Reproduza a Sequência: O jogo irá gerar uma sequência de cores e o jogador deve clicar nos botões na ordem correta.
3. Avançar de Nível: Se o jogador acertar toda a sequência, o jogo aumenta o nível, adicionando mais cores à sequência.
4. Erro ou Vitória: Caso o jogador erre, uma tela de erro será exibida. Caso vença, o jogo exibe uma tela de vitória e permite iniciar um novo jogo.

Estrutura do Código:
Componentes:
- GeniusGame: Componente principal do jogo, que contém a lógica do fluxo de jogo, incluindo os estados do jogo, como sequência, nível, vitória e erro.

Estados:
- sequence: Armazena a sequência de cores gerada.
- playerSequence: Armazena a sequência de cores clicada pelo jogador.
- isPlaying: Controla o início e progresso do jogo.
- level: Controla o nível atual do jogador.
- speed: Controla a velocidade com que a sequência é exibida.
- flashingIndex: Controla qual botão deve piscar durante a exibição da sequência.
- gameWon: Indica se o jogador venceu.
- gameOver: Indica se o jogador errou a sequência.
- difficulty: Armazena a dificuldade do jogo (fácil, médio, difícil).
- maxSequenceLength: Define o comprimento máximo da sequência dependendo da dificuldade.

Funções Principais:
- generateNextStep: Gera um novo passo aleatório para a sequência.
- startGame: Inicializa o jogo com a sequência inicial e reinicia os estados.
- playSequence: Exibe a sequência gerada para o jogador, fazendo os botões piscarem.
- handlePress: Lida com a interação do jogador. Se o jogador clicar no botão correto, a sequência continua; caso contrário, o jogo termina.
- handleDifficulty: Ajusta os parâmetros de dificuldade (sequência máxima e velocidade) de acordo com a escolha do jogador.
- goToDifficultySelection: Retorna para a tela de seleção de dificuldade.

Estrutura da Interface:
- Tela de Dificuldade: O jogador escolhe a dificuldade do jogo (Fácil, Médio, Difícil).
- Tela do Jogo: Exibe os botões coloridos para o jogador interagir e tenta seguir a sequência.
- Tela de Erro: Exibe uma mensagem de erro e permite reiniciar o jogo.
- Tela de Vitória: Exibe uma mensagem de vitória quando o jogador completa o jogo corretamente.

Estilos:
O projeto utiliza o StyleSheet do React Native para aplicar estilos aos componentes, como os botões coloridos, textos, e imagens. Os botões piscam para indicar ao jogador qual botão ele deve pressionar durante o jogo.

O jogo utiliza as seguintes imagens:
- durante.png: Exibida durante o jogo para mostrar que a sequência está em andamento.
- hello.png: Exibida antes do jogo iniciar.
- cry.png: Exibida quando o jogador erra a sequência.
- happy.png: Exibida quando o jogador vence o jogo.

Considerações Finais:
Este projeto oferece uma ótima maneira de praticar programação com React Native e lógica de jogos. Ele também oferece um desafio de memória para os jogadores, com diferentes níveis de dificuldade para tornar o jogo mais interessante.
