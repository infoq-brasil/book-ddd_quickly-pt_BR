# Refatorando para um Conhecimento Profundo
 
## Refatoração Contínua
 
Até agora falamos sobre o domínio e a importância de se criar um modelo que expresse o domínio. Demos algumas orientações sobre as técnicas a serem usadas para criar um modelo útil. O modelo tem que ser bem relacionado ao domínio que o origina. Também dissemos que o projeto do código tem de ser feito em torno do modelo, o qual deve ser melhorado com base nas decisões de projeto. Projetar sem um modelo em mente pode levar a um software que não represente o domínio a que serve, e provavelmente não terá o comportamento esperado. Modelar sem um feedback do design e sem o envolvimento dos desenvolvedores leva a um modelo que não é bem compreendido por aqueles que irão implementá-lo, tornando-se inapropriado às tecnologias utilizadas.
 
Durante o processo de projeto e desenvolvimento, temos que parar de vez em quando para analisar o código, pois pode ser o momento de se fazer uma refatoração. Esse é o processo de redesenhar o código para torná-lo melhor, sem alterar o comportamento da funcionalidade. Geralmente, refatorar é feito em etapas controladas, com muito cuidado para não interromper a funcionalidade ou introduzir algum bug. Afinal, o propósito da refatoração é tornar o código melhor, não pior. Testes automatizados são de grande ajuda para garantir que nada foi corrompido.
 
Há muitas maneiras de refatorar o código. Há inclusive padrões de refatoração. Tais padrões representam uma abordagem automatizada para refatorar. Existem ferramentas construídas sobre tais padrões que tornam a vida do desenvolvedor muito mais fácil do que costumava ser. Sem essas ferramentas, o trabalho tende a ser muito mais difícil. Esse tipo de refatoração se envolve mais com o código e sua qualidade.
 
Há outro tipo de refatoração, relacionado ao domínio e seu modelo. Às vezes há uma nova visão sobre o domínio, algo se tornando mais claro ou uma relação entre dois elementos sendo descoberta. Tudo isso deve ser incluído no projeto através da refatoração. É muito importante ter um código expressivo que seja fácil de ler e compreender. Da leitura do código, alguém deve ser capaz de dizer o que o código faz, mas também o porquê de ele fazer isso. Só então o código realmente capturará a essência do modelo.
 
A refatoração técnica, que é baseada em padrões, pode ser organizada e estruturada. Refatorar para uma análise mais profunda não deve ser feito da mesma maneira, pois não poderemos criar padrões. A complexidade de um modelo e a variedade de modelos não nos oferece a possibilidade de uma abordagem de modelagem de forma mecanicista. Um bom modelo é o resultado de profunda reflexão, introspecção, experiência e talento.
 
Uma das primeiras coisas que são ensinadas sobre modelagem é ler as especificações de negócio procurando por substantivos e verbos. Os substantivos são convertidos em classes, enquanto os verbos se tornam métodos. É uma simplificação que vai levar a um modelo superficial. Todo modelo é assim no início, mas devemos refatorá-lo para uma compreensão cada vez mais aprofundada.
 
O projeto tem que ser flexível. Um projeto rígido resiste à refatoração. O código que não foi construído visando flexibilidade é um código difícil de trabalhar. Quando uma mudança for necessária, você verá o código brigar com você e as coisas que deveriam ser refatoradas tomando muito do seu tempo.
 
Usando um conjunto comprovado de blocos básicos de construção, juntamente com uma linguagem consistente, traz alguma sanidade para o esforço de desenvolvimento. Isso reduz o desafio de encontrar um modelo realmente incisivo, que capta as preocupações sutis dos especialistas do domínio e que pode levar a um design prático. Um modelo que releva o superficial e capta o essencial é um modelo mais profundo. Ele faz com que o software fique em sintonia com o modo de pensar dos especialistas do domínio, sendo mais sensível às necessidades do usuário.
 
Tradicionalmente, refatorar é descrito em termos de transformações no código com motivações técnicas. Refatoração também pode ser motivado por uma visão do domínio e um correspondente refinamento do modelo ou sua expressão no código.
 
Modelos de domínio sofisticados raramente são desenvolvidos sem um processo iterativo de refatoração, incluindo um envolvimento maior dos especialistas do domínio com os desenvolvedores interessados ​​no aprendizado sobre o domínio.


## Trazendo Conceitos-Chave à Tona
<!-- Será que não seria melhor "Revelando conceitos-chave" -->
 
Refatorar é feito em pequenos passos. O resultado é também uma série de pequenas melhorias. Há momentos em que várias pequenas mudanças agregam muito pouco valor para o design, e há momentos em que poucas mudanças fazem uma grande diferença. É um Breakthrough ou uma quebra de barreiras que pressupõe um grande avanço.
 
Começamos com um modelo grosseiro e superficial. Então refinamos o modelo e o design, baseado em um conhecimento mais profundo sobre o domínio, numa melhor compreensão dos conceitos. Adicionamos novos conceitos e abstrações a ele. O design é então reformulado. Cada refinamento adiciona mais clareza ao design. Isso cria, por sua vez, as premissas para um Breakthrough.
 
O Breakthrough muitas vezes envolve uma mudança no pensamento, na forma que vemos o modelo. É também uma fonte de grande progresso no projeto, mas também tem alguns inconvenientes. O Breakthrough pode implicar numa grande quantidade de refatoração. Isso significa tempo e recurso, algo que nunca parece ser suficiente. É muito arriscado, pois uma ampla refatoração pode introduzir mudanças comportamentais na aplicação.
 
Para chegar a um Breakthrough, precisamos fazer com que os conceitos implícitos se tornem explícitos. Quando falamos com os especialistas do domínio, trocamos um monte de ideias e conhecimentos. Alguns dos conceitos fazem o seu próprio caminho para a Linguagem Ubíqua, mas outros permanecem despercebidos no início. São conceitos implícitos, usados para explicar outros conceitos que já estão no modelo. Durante este processo de refinamento do design, alguns desses conceitos implícitos chamam a nossa atenção. Descobrimos que alguns deles desempenham um papel fundamental no design. Nesse ponto, devemos fazer com que esses conceitos se tornem explícitos. Devemos criar classes e relacionamentos para eles. Quando isso acontece, temos chance de vislumbrar um Breakthrough.
 
Conceitos implícitos não devem ficar escondidos. Se eles são conceitos do domínio, devem estar presentes no modelo e no design. Como podemos reconhecê-los? A primeira maneira de descobrir conceitos implícitos é prestar atenção na linguagem que estamos usando durante a modelagem e design, pois contém uma grande quantidade de informações sobre o domínio. No início, pode não ser muito, já que algumas das informações podem não ser usadas corretamente. Alguns dos conceitos podem não ser totalmente compreendidos ou mesmo completamente mal entendidos. Isso tudo é parte do aprendizado de um novo domínio. Mas à medida que construímos a nossa Linguagem Ubíqua, os conceitos-chave fazem o seu caminho até ela. É aí que devemos começar a olhar para os conceitos implícitos.
 
Às vezes, algumas partes do design não são tão claras. Há um conjunto de relações que torna o caminho da computação difícil de ser seguido. Os procedimentos estão fazendo algo complicado que é difícil de entender. Isso é resultado da falta de experiência no design. Esse é um bom lugar para procurar por conceitos escondidos. Provavelmente algo está faltando. Se um conceito chave está faltando no quebra-cabeça, outros vão ter que substituir sua funcionalidade. Isso vai sobrecarregar alguns objetos, adicionando comportamento que não deveria existir. A clareza do projeto estará comprometida. Tente ver se há um conceito ausente. Se for encontrado, torne-o explícito. Refatore o projeto para torná-lo o mais simples e flexível possível.
 
Quando o conhecimento estiver sendo construído, é possível correr em contradições. O que um especialista no domínio diz parece contradizer o que o outro defende. Um requisito pode contradizer outro. Algumas das contradições não são realmente contradições, mas formas diferentes de se ver a mesma coisa ou simplesmente falta de precisão nas explicações. Devemos tentar conciliar a contradição. Às vezes, isso traz à tona importantes conceitos. Mesmo que não, ainda é importante para manter tudo claro.
 
Outra forma óbvia de explorar conceitos do modelo é a utilização da literatura de domínio. Há livros escritos em quase todos os tópicos possíveis. Eles contêm grande quantidade de conhecimento sobre os respectivos domínios. Os livros não costumam conter modelos para os domínios que apresentam. As informações que contêm precisam ser processadas, destiladas e refinadas. No entanto, as informações encontradas em livros são valiosas e oferecem uma visão profunda do domínio.
 
Existem outros conceitos que são muito úteis, quando tornados explícitos: Restrição, Processo e Especificação. Uma Restrição é uma maneira simples de expressar uma invariante. Aconteça o que acontecer aos dados do objeto, a invariante deverá ser respeitada. Isso é feito simplesmente colocando a lógica da invariante em uma Restrição. A seguir um exemplo simples. Seu objetivo é explicar o conceito e não representar a abordagem sugerida por um caso semelhante.
 
 
Podemos acrescentar livros a uma estante, mas nunca devemos acrescentar mais do que a sua capacidade. Isso pode ser visto como parte do comportamento da Estante (Bookshelf), como no código Java abaixo.
 
 
Podemos refatorar o código, extraindo a restrição em um método separado.
 
 
Colocando a restrição em um método separado tem a vantagem de torná-lo explícito. É fácil de ler e todo mundo vai notar que o método add () está sujeito a essa restrição. Há também margem para o crescimento, adicionando mais lógica nesses métodos à medida que a restrição se tornar mais complexa.
 
Processos são geralmente expressos em código com os procedimentos. Não vamos usar uma abordagem procedimental, já que estamos usando uma linguagem orientada a objetos, por isso precisamos escolher um objeto para o processo, e adicionar um comportamento a ele. A melhor maneira de implementar processos é  através da utilização de um Serviço. Se há diferentes maneiras de se realizar o processo, então podemos encapsular o algoritmo em um objeto e usar uma Estratégia. Nem todos os processos devem se tornar explícitos. Se a Linguagem Ubíqua menciona especificamente o respectivo processo, então é hora para uma implementação explícita.
 
A última forma de tornar explícitos os conceitos que estamos abordando aqui é por meio das Especificações. Basta dizer que uma Especificação é utilizada para testar se um objeto satisfaz um determinado critério.
 
A camada de domínio contém regras de negócio que são aplicadas a Entidades e Objetos de Valor. Essas regras são geralmente incorporadas nos objetos a que se aplicam. Algumas dessas regras são apenas perguntas cujas respostas são "sim" ou "não". Tais regras podem ser expressas através de uma série de operações lógicas realizadas em valores Booleanos, sendo o resultado final também um Booleano. Um desses exemplos é o teste realizado em um objeto do cliente para ver se ele está apto para receber determinados créditos. A regra pode ser expressa como um método, chamado isEligible(), implementado no objeto Cliente (Customer). Mas essa regra não é um método simples que funciona estritamente nos dados do cliente. Avaliando-a, percebe-se que ela envolve a verificação de credenciais do cliente, analisando se ele pagou suas dívidas no passado, se ele tem saldos pendentes etc. Tais regras de negócio podem ser grandes e complexas, sobrecarregando o objeto até o ponto que já não servirá a seu propósito original. Nesse ponto, somos tentados a mover a regra inteira para o nível de aplicação, porque parece que se estende além do nível do domínio. Na verdade, é hora de uma refatoração.
 
A regra deve ser encapsulada em um objeto próprio, que se torna a Especificação do Cliente, devendo ser mantida na camada de domínio. O novo objeto irá conter uma série de métodos booleanos que pode testar se um determinado objeto Cliente está apto para o crédito ou não. Cada método tem o papel de um pequeno teste e todos os métodos combinados dar a resposta à pergunta original. Se a regra de negócio não está compreendida em um objeto de Especificação, o código correspondente acabará distribuído por um número de objetos, tornando-se inconsistente.
 
A Especificação é utilizada para testar objetos com o intuito de ver se eles preenchem algum requisito ou se eles estão prontos para algum propósito. Também pode ser usada para selecionar um determinado objeto de uma coleção ou como condição durante a criação de um objeto.
 
Muitas vezes uma única especificação verifica se uma regra simples é satisfeita, só então uma série de Especificações similares são combinadas em uma composição para expressar regras complexas, como esta:
 
 
Testar regras simples é mais fácil, e apenas lendo esse código fica claro o seu significado, qual seja, se um cliente está apto a um reembolso.
