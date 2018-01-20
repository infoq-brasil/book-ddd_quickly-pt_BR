# DDD Importa Hoje: Uma entrevista com Eric Evans
 
InfoQ.com entrevista o idealizador do Domain-Driven Design, Eric Evans, para colocá-lo em um contexto moderno:
 
Por que o DDD é importante hoje e sempre?
 
Fundamentalmente, o DDD é o princípio pelo qual devemos nos concentrar sobre as questões profundas do domínio de nossos usuários. A melhor parte de nossas mentes deve ser dedicada à compreensão desse domínio, colaborando com os peritos no domínio para lutar por uma forma conceitual que possamos usar para construir um software poderoso, flexível.
 
Esse é um princípio que não vai sair de moda. Aplica-se sempre quando estivermos operando em um domínio complexo e intrincado.
 
A tendência de longo prazo é aplicar o software em problemas cada vez mais complexos no coração dessas empresas. Parece-me que essa tendência foi interrompida por alguns anos, quando a web se popularizou. A atenção foi desviada das lógicas ricas e soluções profundas, pois se valorizava apenas obter dados para serem expostos na web, juntamente com comportamentos muito simples. Havia muito disso sendo feito, e publicar coisas simples na web se tornou muito difícil por um tempo, o que absorveu todo o esforço de desenvolvimento.
 
Mas agora que nível básico de uso da web tem sido largamente assimilado, os projetos estão começando a ficar novamente mais ambicioso com relação à lógica de negócios.
 
Muito recentemente, plataformas de desenvolvimento web começaram a amadurecer o suficiente para fazer do desenvolvimento web mais produtivo para o DDD, trazendo uma série de consequências positivas. Por exemplo, SOA, quando bem utilizada, fornece-nos uma forma muito útil de isolar o domínio.
 
Enquanto isso, os processos Ágeis influenciaram bastante, tanto que a maioria dos projetos tem agora pelo menos uma intenção de iteração, trabalha-se em estreita colaboração com parceiros de negócios, aplica-se integração contínua e trabalha-se em um ambiente de grande comunicação.
 
Então o DDD parece ser cada vez mais importante para o futuro próximo, com algumas companhias se estabelecendo.
 
Plataformas tecnológicas (Java,. NET, Ruby, outros) estão em constante evolução. Como o Domain-Driven Design se encaixa nisso?
 
De fato, novas tecnologias e processos devem ser julgados se auxiliarão as equipes a se concentrem no seu domínio em vez de distraí-los dele. O DDD não é específico de uma plataforma tecnológica, contudo algumas plataformas dão formas mais expressivas de criação da lógica de negócios e algumas plataformas têm menos propensão à desordem. Em relação ao depois, os últimos anos sinalizaram uma esperança, principalmente após o fim da terrível década de 90.
 
Java tem sido a escolha padrão dos últimos anos, e quanto à expressividade, é típica de linguagens orientadas a objeto. Quanto à desorganização, a linguagem base não é tão ruim. Tem coleta de lixo, que, na prática, acaba sendo essencial (Em contraste com C++, que exigiu muita atenção a detalhes de baixo nível). A sintaxe Java tem alguma desordem, mas os Plain Old Java Objects (POJOs) ainda podem ser legíveis. E algumas das inovações de sintaxe do Java 5 ajudam na legibilidade.
 
Mas de volta no tempo, quando os primeiros frameworks J2EE foram lançados, montanhas de código de framework sepultaram a expressividade básica. Seguir as convenções antigas produzia objetos horríveis (tais como EJB Home, assessores prefixados para todas as variáveis do tipo get / set etc). As ferramentas eram tão complicadas que absorviam toda a capacidade das equipes de desenvolvimento só para fazê-las funcionar. Era tão difícil de mudar tais objetos, devido à grande confusão de código gerado e no XML atrelado, que as pessoas simplesmente não alteravam muito. Essa foi uma plataforma que fez a efetiva modelagem de domínio se tornar quase impossível.
 
Combine isso com a imperatividade para produzir interfaces Web mediadas por http e html (que não foram concebidas para isso) usando ferramentas bastante primitivas. Durante esse período, criar e manter uma UI decente se tornou tão difícil que pouca atenção foi deixada para o design de complexas funcionalidades internas. Ironicamente, no momento em que a tecnologia de objetos despontou, a modelagem e o design sofisticados foram fortemente atingidos.
 
A situação foi semelhante na plataforma .Net, com algumas questões sendo tratadas um pouco melhor, e outras um pouco pior.
 
Foi um período desanimador, mas a tendência mudou nos últimos quatro anos. Primeiro, olhando para Java, tem havido uma confluência de uma nova sofisticação na comunidade sobre como usar frameworks de forma seletiva, e uma mistura variada de novos frameworks (principalmente de código aberto) que são cada vez mais melhorados. Frameworks como Hibernate e Spring lidam com trabalhos específicos que o J2EE buscou atender, mas de uma forma muito mais leve. Abordagens como AJAX, tentam resolver o problema de interface com o usuário de uma maneira menos trabalhosa. Os projetos são muito mais inteligentes agora, escolhendo os elementos do J2EE que agregarão valor, misturando-os com alguns desses elementos mais novos. O termo POJO foi cunhado durante essa época.
 
O resultado é uma diminuição gradual, mas perceptível, no esforço técnico dos projetos, com uma clara elevação do isolamento da lógica de negócios em relação ao resto do sistema, para que eles possam ser escritos como POJOs. Isso não significa produzir automaticamente domain-driven design, mas torna-o uma oportunidade concreta.
 
Esse é o mundo Java. Então você tem as recém-chegadas linguagens como Ruby, que possui uma sintaxe muito expressiva, sendo, neste nível básico, uma linguagem muito boa para DDD (embora eu ainda não tenha ouvido falar de muita utilização prática nesses tipos de aplicações). Rails tem gerado muita expectativa porque finalmente parece facilitar a criação de interfaces de usuário Web tão facilmente quanto as UIs desktop no início dos anos 90, antes da Web. Ultimamente, essa capacidade tem sido bastante aplicada na construção de algumas das grandes aplicações Web que não têm por trás tanta riqueza no domínio, já que até mesmo elas foram dolorosamente difíceis de ser concebidas no passado. Mas minha esperança é que, como a parte do problema referente à implementação da UI é reduzida, as pessoas verão isso como uma oportunidade para concentrar ainda mais sua atenção no domínio. Se o uso de Ruby começar a sempre ir nessa direção, acredito que poderia ser uma excelente plataforma para o DDD. (A infraestrutura de algumas peças provavelmente teria que ser construída).
 
O que está despontando são os esforços na área de linguagens específicas de domínio (DSLs), que há muito eu acreditava ser o próximo grande passo para o DDD. Até hoje, ainda não se tem uma ferramenta que realmente nos dê o que precisamos. Mas as pessoas estão experimentando mais do que nunca essa área, e isso me faz esperançoso.
 
Agora, tudo o que posso dizer é que a maioria das pessoas que tentam aplicar o DDD estão trabalhando com Java ou .Net, algumas com Smalltalk. Por isso, é uma tendência positiva no mundo Java que está tendo o efeito imediato.
 
O que está acontecendo na comunidade DDD desde que você escreveu o seu livro?
 
Uma coisa que me excita é quando as pessoas aplicam os princípios falados em meu livro, utilizando-os de maneira que eu nunca esperava. Um exemplo é o uso do design estratégico na StatOil, uma empresa norueguesa de petróleo. Os arquitetos escreveram um relato de experiência sobre o assunto. (Você pode lê-lo em http://domaindrivendesign.org/articles/)
 
Entre outras coisas, eles se basearam no mapeamento de contexto para ser aplicado numa avaliação entre um software de prateleira em construção ou comprar decisões.
 
Como um exemplo bastante diferente, alguns de nós exploramos diversas questões no desenvolvimento de uma biblioteca de código Java com alguns objetos de domínio fundamentais, necessários para muitos projetos. Pode-se verificar isso em:
 
http://timeandmoney.domainlanguage.com
 
Nós exploramos, por exemplo, o quão longe se pode avançar na ideia de ter uma linguagem específica de domínio fluente, enquanto ainda implementamos os objetos em Java.
 
Muita coisa está acontecendo lá fora. Eu sempre aprecio quando pessoas entram em contato comigo para contar sobre o que estão fazendo.
 
Você tem algum conselho para quem está tentando aprender DDD hoje?
 
Leia o meu livro! ;-) Além disso, tente usá-lo no seu projeto. Um dos nossos objetivos iniciais foi o de fornecer um bom exemplo com o qual as pessoas pudessem aprender na prática.
 
Um aspecto a se ter em mente é que, em grande parte, o DDD é algo que as equipes tem de fazer, então você precisa ser um evangelista. Sendo bem realista, você pode querer buscar um projeto onde já se tenha um esforço para fazer isso.
 
Tenha em mente algumas das armadilhas de modelagem de domínio:
 
1) Ponha a ‘mão na massa’. Modeladores necessitam de código.
 
2) Concentre-se em cenários concretos. Pensamento abstrato tem que ser ancorado em casos concretos.
 
3) Não tente aplicar o DDD em tudo. Desenhe um mapa de contexto e decida sobre onde você vai ou não fazer um esforço para usar o DDD. Então não se preocupe com estar fora desses limites.
 
4) Experimente muito e espere fazer muitas besteiras. A modelagem é um processo criativo.
 
## Sobre Eric Evans
 
Eric Evans é autor de "Domain-Driven Design: Combater a Complexidade do Software", Addison-Wesley 2004.
 
Desde o início de 1990, ele trabalhou em muitos projetos de desenvolvimento de sistemas para grandes empresas, contendo muitos objetos com diversas abordagens e muitos resultados diferentes. O livro é uma síntese dessa experiência. Apresenta um sistema de modelagem e técnicas de design que as equipes bem-sucedidas têm utilizado para alinhar complexos sistemas de software com as necessidades do negócio, mantendo projetos ágeis à medida que o sistema cresce.
 
Eric agora lidera "Linguagem de Domínio", um grupo de consultoria que treina equipes na aplicação do domain-driven design, ajudando-os a fazer o seu trabalho de desenvolvimento mais produtivo e mais valioso para os seus negócios.
 
### Nossos Serviços
 
Ajudamos ambiciosos projetos de software a perceberem o potencial do domain-driven design e processos ágeis.
 
Para fazer a modelagem de domínio e design realmente funcionarem num projeto, é exigido que o design de alto nível e detalhados venham juntos. É por isso que oferecemos uma combinação de serviços que podem realmente fazer o processo de domain-driven design surgir do zero.
 
Nossos cursos de treinamento e mentores fortalecem as habilidades básicas da equipe na modelagem e implementação de um código efetivo. Nossos treinadores focam nos esforço da equipe e mitigam falhas no processo que entravam o design do sistema mais significativo para o negócio. Nossos consultores de design estratégico abordam os problemas que afetam a trajetória de todo o projeto, facilitando o desenvolvimento de um grande framework que auxilia o desenvolvimento e conduz o projeto para atingir os objetivos da organização.
 
## Começe uma Avaliação
 
A avaliação que faremos dará não somente perspectivas como também recomendações concretas. Esclareceremos onde você está agora, para onde você quer ir e começaremos a desenhar um roteiro de como chegar a esse objetivo.
 
Para Agendar uma Avaliação
 
Para preços, horários e mais informações, ligue para 415-401-7020 ou escreva para info@domainlanguage.com.
 
 
www.domainlanguage.com
 
