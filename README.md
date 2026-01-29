# Trabalho de Redes de Computadores (RC)
Grupo : Alexandra Victoria Azevedo Araujo, Aline Barros dos Anjos, Emanuela Maria Cavalcanti Alves, Iris de Souza Kemper e Jeovana Bernardino da Silva
3º T.I-M

Descrição do jogo : Este projeto traz uma versão do jogo Pedra, Papel e Tesoura, desenvolvida em Java utilizando um modelo cliente-servidor. Com comunicação via sockets TCP, ele permite que três jogadores participem ao mesmo tempo, com todos conectados a um servidor central que gerencia as regras e a dinâmica da partida. Assim, você pode competir em tempo real com os seus amigos.

Como executar o projeto : há duas maneiras desse projeto ser executado, as maneiras são as seguintes :
1º maneira : 
Primeiro, localize a pasta principal do seu jogo no computador. Depois, abra o Prompt de Comando (ou terminal). 
No terminal, use o comando cd para navegar até a pasta `bin` do projeto, onde estão os arquivos compilados. Por exemplo: 
cd C:\Users\user\eclipse-workspace\PedraPapelTesoura_Redes\bin

Uma vez na pasta bin, você pode iniciar o jogo com o seguinte comando:
java jogo.cliente_TCP
Cada vez que você executa esse comando em um novo terminal, um novo jogador é adicionado ao jogo. Assim, cada terminal aberto representa um jogador diferente participando da partida.

2º maneira :
Um computador atua como servidor, e para encontrar o IP da máquina, você pode usar o comando ipconfig no CMD. Esse IP, junto com a porta, deve ser inserido no código dos clientes, já que a comunicação é feita via TCP.
Depois de configurar tudo, inicie o servidor. Em computadores diferentes, cada cliente é executado pelo Eclipse, e cada nova execução representa um jogador diferente. Assim, todos podem se conectar e jogar juntos. 

Como jogar : 
- Primeiro, o servidor é iniciado e fica aguardando três conexões.
- Cada jogador executa o cliente e recebe um número de identificação.
- Quando todos estiverem conectados, cada jogador deve digitar PRONTO para iniciar.
- O jogo possui 5 rodadas.
- Em cada rodada, os jogadores escolhem:
    - 1 Pedra
    - 2 Papel
    - 3 Tesoura
- O servidor verifica o resultado seguindo as regras do jogo.
- Quem vencer a rodada ganha 1 ponto.
- Em caso de empate, ninguém pontua.
- Ao final de cada rodada, o placar é exibido.
- Após a quinta rodada, o jogo é encerrado e o servidor fecha as conexões.



