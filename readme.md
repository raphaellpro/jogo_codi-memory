<h1 align="center"> Projeto Codi Memory Game </h1>


<p align="center">
<img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge"/>
</p>

# Índice 

- [Índice](#índice)
- [Descrição do Projeto](#descrição-do-projeto)
- [Funcionalidades e Demonstração da Aplicação](#funcionalidades-e-demonstração-da-aplicação)
- [Tecnologias e sites utilizados](#tecnologias-e-sites-utilizados)
- [Desenvolvimento](#desenvolvimento)
- [Conclusão](#conclusão)


# Descrição do Projeto

<p align="justify">Este jogo foi produzido com a utilização de alguns conceitos básicos de HTML5, CSS3 e Javascript. Dessa forma, foi pensado para ser o jogo da memória da Escola Codi Academy. Foram trabalhados eventos, funções, arrays, métodos, comparações, entre outras funcionalidades e operações. O jogo foi intitulado como: Codi Memory Game.</p>

# Funcionalidades e Demonstração da Aplicação

# <h3>Tecnologias e sites utilizados</h3>

<p align="left">Pesquisas e verificação do funcionamento do código:  Navegador de Internet Google Chrome</p>
<p align="left">Pesquisas e verificação do funcionamento do código: https://www.microsoft.com/pt-br/edge</p>
<p align="left">Edição/produção do código: Visual Studio Code - Code Editing. Redefined</p>
<p align="left">Escolha de cores e seus respectivos códigos HEX: HTML Color Codes 🎨</p> 
<p align="left">Consulta: JavaScript: The Definitive Guide</p> 
<p align="left">Consulta: Appendix B. Keyboard Key Code Values</p>
<p align="left">Consulta: https://developer.mozilla.org/pt-BR/docs/Web/CSS/flex-wrap</p>
<p align="left">Consulta: Document: DOMContentLoaded event - Web APIs | MDN</p> 
<p align="left">Consulta: https://medium.com/code-sketch/jogo-da-memoria-em-vanilla-javascript-6129e5eac7a5</p> 
<p align="left">Extensão utilizada no VS Code: Live Server (https://github.com/ritwickdey/live-server-web-extension)</p>
<p align="left">Aula: https://codiacademy.com/cursos/desenvolvimento-web-front-end-completo-com-8-linguagens-frameworks/lessons/p3-3-codi-memory-conferindo-cards/</p> 


# <h3>Desenvolvimento</h3>

<p align="justify">Foram inseridos os documentos padrões (index.html, style.css, script.js, readme.md)  com a devida base inicial para funcionamento no navegador Google e Edge, nas versões mais atuais.
Além das instruções repassadas nas aulas, foram realizadas algumas alterações simples, como: estilização e reposicionamento simples com CSS e pequena alteração na estrutura básica do HTML.</p>

1) Inicialização do Jogo:

<p align="justify">A inicialização do jogo ocorre quando o evento DOMContentLoaded é acionado, garantindo que o HTML foi completamente carregado antes de executar o script. Dentro desse evento, a função “createBoard” é chamada para criar a grade de cartões na tela.</p>

2) Configuração das Variáveis:

<p align="justify">“cardArray”: matriz que contém objetos representando os cartões do jogo, cada objeto possui um nome (name) e um caminho para a imagem (img).
“grid”: referência ao elemento HTML com a classe “grid”, onde os cartões serão exibidos.
“resultDisplay”: referência ao elemento HTML com o id “result”, que exibirá o número de pares encontrados.
“cardsChosen”: Um array para armazenar os nomes dos cartões escolhidos pelo jogador.
“cardsChosenId”: Um array para armazenar os IDs dos cartões escolhidos pelo jogador.
“pares”: Um array para armazenar os pares de cartões que foram correspondidos.</p>

3) Controles do Jogo:

<p align="justify">click EventListener: Cada cartão na grade possui um evento de clique (click) associado à função “flipCard”, que é responsável por virar o cartão.</p>


4) Funcionamento do Jogo:

<p align="justify">createBoard(): Essa função é responsável por criar a grade de cartões na tela. Ela utiliza um loop para criar elementos “img” para cada cartão e os adiciona à grade.
flipCard(): Acionada quando um cartão é clicado. Ela vira o cartão exibindo a imagem associada e adiciona o nome e o ID do cartão aos arrays “cardsChosen” e “cardsChosenId”, respectivamente. Quando dois cartões são virados, a função “checkforMatch” é chamada.
checkforMatch(): Esta função verifica se os dois cartões virados formam um par ou não. Se formarem um par, os cartões permanecem virados, e os eventos de clique são removidos. Se não formarem um par, os cartões são virados de volta. Em ambos os casos, o jogador recebe uma mensagem adequada ao evento. O número de pares encontrados é exibido no placar e se o jogador encontrar todos os pares, uma mensagem de parabéns é exibida.
setTimeout(): É usado para dar um intervalo de 500 milissegundos antes de chamar a função “checkforMatch”. Isso permite que o jogador veja os cartões virados antes de serem verificados.
Essa lógica geral cria um jogo de memória onde o jogador deve encontrar todos os pares correspondentes virando os cartões na tela. O jogo continua até que todos os pares sejam encontrados.</p>

# <h3>Conclusão</h3>

<p align="justify">A produção desse projeto mostrou a importância do uso das variáveis e da aplicação do conceito de objetos e as devidas manipulações, com mais utilização do HTML e CSS, em comparação com os 2 projetos anteriores. É necessário se atentar ao comportamento do grid na página e o posicionamento dos objetos (no grid) que queremos inserir em um jogo, por exemplo. O uso de constantes, das funções “checkforMatch” e “Math.random()” foram muito importantes para o projeto, quando o objetivo foi gerar cards em posições aleatórias e checar se eram iguais, não utilizadas isoladamente, mas em conjunto com o restante do código.
As oportunidades deste projeto são: melhorar a responsividade do jogo em relação aos diversos tamanhos de tela; aperfeiçoar o código para possibilitar que o usuário jogue em seu smartphone; implementar sistema de pontuação mais complexo (de acordo tempo para encontrar todos os pares, por exemplo); implementar botões de Play, Restart e Pause; e melhorar a interface (UX/UI).
O jogo está funcionando e foram feitos testes no Google Chrome e no Microsoft Edge.
</p>


