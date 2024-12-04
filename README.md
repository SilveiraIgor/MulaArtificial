# Como usar:

Para quem só tá querendo usar o programa, siga os seguintes passos:
1. Clique no botão verde escrito "Code" e "Download Zip".
2. Extraia o .rar chamado MulaArtificial-main, depois extraia o .rar chamado Mula.
3. Abra a pasta Mula.
4. Abra o Times.txt e verifique se estão os times da fase que você quer simular. Essa parte é editável, se quiser simular uma configuração diferente é só mudar o nome do time ou a seed dele (o número ao lado do nome). <b> A última linha desse txt deve ser um começo de linha sem nada escrito. </b>
5. Abra o Conhecimento.txt e coloque quem você acha que ganha de quem no formato: Time1 > Time2 (Time1 ganha do Time2 --- maiores informações em 03/12/24: Segunda Versão). Salve as suas modificações.  <b> A última linha desse txt deve ser um começo de linha sem nada escrito. </b>
6. Execute o MulaArtificial, espere 5 segundos e a simulação vai começar a ser exibida. Para dar um exemplo de como eu usei, assista uns pedaços do vídeo https://youtu.be/4GtwHQ-7srU, a versão atual do MulaArtificial será diferente da do video, para maiores informações leia o Mudanças.

# Videos: 
Uma breve explicação sobre o funcionamento & objetivo do programa pode ser encontrado em: https://youtu.be/uor9v8o8XJs

O video simulando o Legends que talvez ajude a entender como funciona a segunda versão: https://youtu.be/4GtwHQ-7srU

# Para os programadores:
Já aviso de antemão que o projeto inteiro foi feito em menos de um final de semana, então o código não está nem otimizado e nem bonito.

Se mesmo assim você quiser ver o que tá rolando, dentro do rar terá 4 arquivos Python:
- CoreSystem.py, que é o arquivo principal para rodar o código.
- LeitorTimes.py, que lê os times e também define a classe Equipe.
- LeitorConhecimento.py, que só lê o conhecimento, ela tem espaço para crescer para facilitar certas coisas.
- Round.py, que controla tudo que acontece num round e também o que é um confronto. Esse é o arquivo mais importante.

# Mudanças:
### 04/12/24: Terceira Versão
A tela começa já em um tamanho que aparece a tabela inteira, então não precisa ficar reajustando o tamanho.

Quando o programa termina de computar, agora ele mostra todas as partidas que aconteceram que não estão na base de conhecimento.

Se o programa ainda estiver computando e você salvar alguma alteração no Conhecimento.txt, então o programa começa a rodar novamente do zero com o novo conhecimento. Essa alteração foi feita porque era chato ficar fechando e abrindo novamente.

### 03/12/24: Segunda Versão
Essa é a versão do segundo vídeo.

Mudei a tabela das estatísticas para ser mais fácil de ver as linhas e colunas.

Adicionei um pouco de inferencia em linguagem natural sobre o Conhecimento.txt, agora é possível fazer tipo:
1. Furia > Wildcard (Furia ganha de Wildcard)
2. Furia > Wildcard 3DMAX Big (Furia ganha de todos os times elencados depois do >, podendo ter qualquer quantidade de times)
3. Todos > Furia (Todas as equipes ganham da Furia)
4. Furia > Todos (Furia ganha de todos os times)
5. Furia > Todos - NaVi G2 (Furia ganha de todos os times, menos da NaVi e da G2, depois do - pode vir qualquer número de times)
6. Todos - NaVi G2 > Furia (Todos menos a NaVi e a G2 ganham da Furia, entre o - e o > podem ter qualquer quantidade de times)



### 02/12/24: Primeira Versão 
O programa base, igual está no primeiro vídeo.  
