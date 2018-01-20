# Criando uma Linguagem Ubíqua
 
<!-- TODO revisar a traduação inteira -->

Como podemos começar a construir uma linguagem? Mostraremos um diálogo hipotético entre um desenvolvedor de software e um especialista de domínio no projeto de monitoramento de tráfego aéreo. Atente para as palavras que aparecem em negrito.
 
Desenvolvedor: Queremos monitorar o tráfego aéreo. Por onde começamos?
 
Especialista: Vamos começar do básico. Todo esse tráfego é formado por aviões. Cada avião decola a partir de um __local de partida__ e aterrissa em um __local de destino__.
 
Desenvolvedor: Isso é fácil. Quando se voa, o avião pode apenas escolher qualquer caminho aéreo que os pilotos quiserem? São eles que decidem qual caminho seguir, desde que alcancem o destino?
 
Especialista: Oh, não. Os pilotos recebem uma rota que deve seguir. E eles devem ficar o mais próximo possível nessa rota.
 
Desenvolvedor: Estou pensando nessa __rota__ como um ponto 3D no ar. Se usarmos um sistema de coordenadas cartesianas, então a __rota__ seria simplesmente uma série de pontos 3D.
 
Especialista: Eu não penso assim. Não vejo a __rota__ dessa maneira. A realmente é rota a projeção no chão do caminho feito pelo avião no ar. A __rota__ passa por uma série de pontos no solo determinados pela sua latitude e longitude.
 
Desenvolvedor: OK. Então chamaremos cada um desses pontos de __fixo__, porque é um ponto fixo na superfície da Terra. Vamos usar, então, uma série de pontos 2D para descrever o caminho. E, a propósito, a __partida__ e o __destino__ são apenas __fixos__. Não devemos considerá-los como conceitos distintos. A rota alcança seu destino, uma vez que atinge qualquer outro __fixo__. O avião deve seguir a rota, mas isso significa que ele pode voar tão alto ou tão baixo como quiser?
 
Perito: Não. A altitude que um avião deve ter em um determinado momento é também estabelecida no plano de voo.
 
Desenvolvedor: __Plano de voo__? O que é isso?
 
Especialista: Antes de deixar o aeroporto, os pilotos recebem um detalhado plano de voo, que inclui todos os tipos de informações sobre o voo: a __rota__, __altitude__ de cruzeiro, a __velocidade__ de cruzeiro, o tipo de __avião__, até mesmo informações sobre os membros da tripulação.
 
Desenvolvedor: Hmm, o __plano de voo__ parece muito importante para mim. Vamos incluí-lo no modelo.
 
 
Desenvolvedor: Assim está melhor. Agora que eu estou olhando para ele, percebo uma coisa. Quando estamos monitorando o tráfego aéreo, não estamos realmente interessados ​​nos aviões em si, se são brancos ou azuis, se são Boeing ou Airbus. Estamos interessados ​​em seu __voo__. Isso é o que realmente estamos buscando e medindo. Acho que devemos mudar o modelo um pouco para que seja mais preciso.
 
Observe como essa equipe, falando sobre o domínio de monitoramento do tráfego aéreo e em torno de seu modelo incipiente, está lentamente criando uma linguagem formada pelas palavras em negrito. Além disso, observe como ela muda o modelo!
 
No entanto, na vida real, tal diálogo é muito mais detalhado e as pessoas muitas vezes falam de coisas indiretamente, entram demasiadamente em detalhes ou escolhem os conceitos errados, o que pode ocasionar numa linguagem muito difícil de ser compreendida. Para começar esse tipo de trabalho, todos os membros da equipe devem estar cientes da necessidade de se criar uma linguagem comum, devendo sempre ser lembrados de manter o foco no que for essencial, e usar a linguagem sempre que necessário. Devemos reduzir ao mínimo o uso do nosso próprio jargão durante tais sessões, e usar sempre a Linguagem Ubíqua, pois isso nos ajudará a comunicar de forma clara e precisa.
 
É altamente aconselhado aos desenvolvedores que implementem os principais conceitos do modelo no código. Uma classe pode ser criada para a Rota e outra para o Fixo. A classe Fixo poderia herdar de uma classe 2DPoint, ou pode conter um 2DPoint como seu principal atributo. Isso depende de outros fatores que serão discutidos mais tarde. Criando classes para os conceitos do modelo correspondente, estaremos fazendo o mapeamento entre o modelo e o código, e entre a linguagem e o código. Isto é muito útil, pois faz com que o código se torne mais legível, reproduzindo, de fato, o modelo. Fazer com que o código expresse o modelo compensará mais tarde no projeto, quando o modelo crescer e as alterações no código levarem a consequências indesejáveis, caso não tenha sido devidamente projetado.
 
Vimos como a linguagem é compartilhada por toda a equipe e também como ela ajuda a construir conhecimento e criar o modelo. O que devemos usar para a linguagem? Apenas o discurso? Nós usamos diagramas. O que mais? Escrita?
 
Alguns podem dizer que a UML é boa o suficiente para construir um modelo. E, de fato, é uma ótima ferramenta para anotar conceitos-chave como classes e para expressar as relações entre elas. Você pode desenhar quatro ou cinco classes sobre um bloco de desenho, anotar seus nomes, e mostrar as relações entre elas. É muito fácil para que todos possam acompanhar o que você está pensando. Uma expressão gráfica de uma ideia é fácil de ser entendida. Todos, instantaneamente, compartilharão a mesma visão sobre um determinado tema, tornando-se mais simples a comunicação com base nisso. Quando novas ideias surgirem, o diagrama deverá ser modificado para refletir a mudança conceitual.
 
Diagramas UML são muito úteis quando o número de elementos envolvidos é pequeno. Mas a UML pode crescer como cogumelos depois de uma chuva de verão agradável. O que você faz quando você tem centenas de classes enchendo uma folha de papel tão grande quanto o Mississippi? É difícil de ler até mesmo pelos especialistas em software, sem mencionar os especialistas do domínio. Eles não vão entender muito quando o diagrama crescer, algo que acontece mesmo para projetos de médio porte.
 
Além disso, a UML é boa para representar as classes, seus atributos e as relações entre eles. Mas o comportamento das classes e suas restrições não são tão facilmente expressos. Para isso, a UML prevê textos colocados como notas nos diagramas. Então a UML não pode transmitir dois aspectos importantes de um modelo: o significado dos conceitos que representa e o que objetos devem fazer. Mas isso é o de menos, já que podemos acrescentar outras ferramentas de comunicação para fazê-lo.
 
Podemos usar documentos. Uma maneira conveniente de se comunicar o modelo é fazer com que alguns poucos diagramas contenham um pequeno subconjunto do modelo. Esses diagramas conteriam várias classes e a relação entre elas. Isso já inclui uma boa parte dos conceitos envolvidos. Então, podemos adicionar textos ao diagrama. O texto vai explicar o comportamento e restrições, algo que o diagrama por si só não consegue. Cada subseção tentará explicar um aspecto importante do domínio, direcionando um "holofote" para iluminar uma parte do domínio.
 
Esses documentos podem ser até mesmo desenhados à mão, porque isso transmite a sensação de que eles são temporários, podendo ser alterados em um futuro próximo, o que é verdade, pois o modelo mudou muitas vezes no início, antes que ele atingisse a estabilidade.
 
Pode ser tentador tentar criar um diagrama grande abarcando o modelo inteiro. No entanto, na maioria das vezes tais diagramas são quase impossíveis de serem juntados em um único. E, além disso, mesmo que você tenha sucesso em fazer tal diagrama unificado, ele será tão confuso que não transmitirá o entendimento melhor do que uma coleção de diagramas de pequeno porte o faz.
 
Desconfie de documentos longos. Leva muito tempo para escrevê-los e eles podem se tornar obsoletos antes que estejam acabados. Os documentos devem estar em sincronia com o modelo. Documentos antigos, usando a linguagem errada, não refletem o modelo e não são muito úteis. Tente evitá-los quando possível.
 
Também é possível se comunicar usando o código. Essa abordagem é amplamente defendida pela comunidade XP. Código bem escrito pode ser muito comunicativo. Embora o comportamento expresso por um método seja claro, será que o nome do método é tão claro quanto o seu corpo? Assertivas de um teste falam por si, mas e sobre os nomes de variáveis ​​e a estrutura geral do código? Eles estão dizendo a história toda, em alto e bom som? Um código, que funcionalmente faz a coisa certa, não necessariamente expressa tal coisa da melhor forma. Escrever um modelo no código é muito difícil.
 
Há outras maneiras de se comunicar durante o projeto. Este livro não tem o propósito de apresentar todas elas. No entanto, uma coisa fica clara: a equipe de projeto, composta por arquitetos de software, desenvolvedores e especialistas de domínio, precisa de uma linguagem que unifica suas ações, com o objetivo de ajudá-los a criar um modelo e expressar esse modelo através do código.
