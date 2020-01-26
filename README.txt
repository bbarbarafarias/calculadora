Calculadora simples que realiza operações apenas com dois termos; 

Primeiro declare o título com nome CALCULADORA;   

Na linha 125 foi declarado o identificador calculador, dentro da tag <texarea> foi colocado um display utilizando a tag <textarea> para edição da caixa de texto; 

O disabled foi colocado para a caixa de texto não ser editada; 

disabled rows="1" quer dizer que a caixa de texto só vai ter uma linha; 

A partir da linha 125 foi definido os botões de número e operadores da calculadora que possui 4 linhas e cada linha possui 4 botões, para cada linha foi necessário declarar uma <div>, serve para alterar o estilo em partes específicas da página e posicionar objetos; 

Voltando para linha 07 foi declarado o estilo para receber o css; 

O primeiro estilo feito foi o body que é o corpo que inclui: borda para conseguir visualizar a caixa do body; 

O CSS e a folha de estilo da nossa calculadora, nela vamos definir a aparência usando a marcação 

Vamos trabalhar por blocos, o primeiro que vamos inserir será definido o corpo da calculadora (body) que é o conteúdo do nosso HTML;  

No body vamos definir:  largura, posição altura e margem esquerda;  

Definindo o body, vamos para #calculadora 

Na #calculadora vamos definir: borda, cor do background, largura, altura, preenchimento, borda lateral e a margem;  

Finalizando essa parte vamos definir os botões;  

Vamos definir os botões em: largura, altura, tamanho da fonte, preenchimento;  

Bom declarei as cores em PX porque está relacionada ao tamanho da fonte atual nem a unidades absolutas, e também declarei em vetor; 

Com isso a parte de Css foi finalizada, já definimos a aparência da calculadora; 

Durante o código resolvi mudar os parâmetros do botão de igual, então dentro da tag <button>, inseri o style com a largura de 215px; 

Alterei as cores dos botoes C e = para cor salmão;  

Da linha 45 até 118 será a parte do Java Script;  

A primeira variável e a “numDisplay que vai receber uma string vazia (elemento de texto);  

Depois foi declarada uma função que vai ser chamada sempre quando os botes de número forem pressionados, declarei a função como pressNum. 

Voltando para linha 47 declarei a variável como número vazio;  

Na função “pressNum”, coloquei número =num.innerHtml, que e o número que vem do botão; Depois coloquei um console do número, para verificar se o valor está correto; 

No console vai mostrar o que está salvo na variável número;  

Agora volte na linha a partir do 125, para inserir o número nos botões para chamar a função;  

Colocar onclick em todos os botões para chamar a função pressNum que está declarando a função, foi configurado todos os botões de número, o ponto de ponto também foi configurado porque também é um número.  

Voltando na função pressNum, vai concatenar os valores anteriores com os antecedentes; 

Acrescentei na função o concat que vai concatenar o que já foi salvo, e salvo na variável número e depois exibir;  

Na linha 95 criei a função limpar memoria que vai trazer a variavel número, e atribuir o valor inicial vazio. Qualquer número ela vai apagar; 

A função limparMemoria vai ser chamada quando o botão C limpaTela for clicado; 

Na linha 110, declarei a função “exibirTela”, pegar o que está  no (numDisplay) vou concatenar, para quando um botão for pressionado o número também deve ser concatenado na tela do display;  

A var tela que vai no documento tem a função de procurar um elemento pelo seu identificador (ID) chamado display; 

Quando chamar a função "exibirTela" o conteúdo deve ser exibido no display; 

O conteúdo vai ser exibido toda vez que clicar no botão, tenho que editar a função pressionaNum, tiro do console e adicione na function exibirTela; 

Ao testar percebi que estava concatenando 2 vezes, está concatenando na função "pressionaNum e na função "exibirTela" 

Para corrigir à falha foi necessário colocar o número interno no botão na função "exibirTela"; 

Agora no botão AC que tem a função de limpar a tela, foi criada uma function limparTela. Essa função vai limpar o "numDisplay e "limparMemoria" do console; 

Para o botão AC funcionar, precisa chamar ele no botão limpar tela;  

E para limpar a tela e a memória foi criada a função "limpaTudo"; 

E preciso chamar essa função no botão AC; 

Para o botão de operador funcionar, necessário declarar a function pressionaOperador, vou adicionar na função os operadores; 

Foi criado um vetor chamado termos que vai armazenar os termos da operação; 

Considere que a operação tem 3 termos (número e operador); 

Esse vetor vai ter 3 espaços, que estão vazios (primeiro termo, operador e segundo termo); lembrando que as casas são numeradas de 0 em diante;  

Deve deixar os espaços como indefinido; 

Quando clicar no botão operador o termo 0 ele precisa ter o valor salvo no número (memória interna); 

No segundo termo[1] que corresponde ao operador, ele vai ser passado pela parâmetro da função; 

Por fim colocando a função "exibirTela 

Colocar a função "PressionaOperador nos botões de operadores e passar o proprio botão como parâmetro; 

O termo[2] ainda está indefinido; 

Pressione o botão de operador essa função tem que apagar quando pressiona o botão de operador; 

Na função "pressioneOperador" adicione número=""; 

Declare a function pressEqual, para pressionar o botão de igualde deve adicionar o termos[2] que e o terceiro elemento  do vetor e seja preenchido com número que está na var número; 

Necessário chamar a função pressEqual no botão de igualdade para realizar a soma no botão de igualdade (pressEqual);  

Crie uma variavel para o resultado que deve estár indefinida; 

Volte para função pressEqual declare o resultado sendo igual ao termos[0] + termos[2], depois mostre o resultado na tela; 

Mas antes de mostrar o resultado e necessário que limpe o display, portanto coloque a função "limparTela".  

Na função pressEqual transforme os termos em números, inserindo a classe Number na frente de cada termos; 

Agora precisamos identificar qual operação será realizada, nesse caso utilizamos switch case. O break associada com cada case garante que o programa saia da condicional switch assim que a instrução correspondente for executada e executa a instrução que segue logo após o switch. Caso switch termos[1] seja igual '+' o resultado vai ser operação de soma insira o break para sair do loop. Realize um switch case para cada operador;  

Para limpar o console precisa ir na função "LimparMemoria" necessário colocar os termos como indefinido, e o resultado como indefinido também;  

Para continuar com o cálculo depois que ele exibe o resultado, precisa escolher uma operação para calcular com o resultado. Precisa ir na função "pressEqual" e criar uma variavel "manterNumero"; O "manterNumero" precisa ser declarado antes do "limparTudo"; 

Agora precisamos colocar algumas restrições, como limitar os operadores para não se repetir várias vezes;  

Para isso na função "pressionaOperador" vamos colocar uma condição IF se ele estiver indefinido ele precisa ser definido, se ele já estiver definido não precisa declarar porque fora da condição nada acontece;   

Para limitar o uso do botão de igual, precisa adicionar o if na função pressEqual. Se deseja usar o botão de igual se o termo zero estiver preenchido, ou seja, se ele for diferente de indefinido aparece uma mensagem de falha, o termo do meio do operador estiver preenchido ou seja se ele for diferente de indefinido e se o numDisplay também estiver preenchido, Se for diferente de vazio; Portanto o botão de igual só vai realizar essa função se tiver um primeiro termos de operação o segundo termos que e o operador (linha 68)  e se o NumDisplay  tiver algum número, o NumDisplay e o terceiro termos, caso contrário não realiza nenhuma função; 

Ao realizar o teste percebi que teve um erro ao colocar o ponto, porque os números não estão em formato de número, para corrigir à falha precisa deixar em formato de string, a falha foi corrigida na linha 91;  

Realize o teste.   

Acabou!!! ^^  

 

 

  

 

 

 

 

 

 

 

 
