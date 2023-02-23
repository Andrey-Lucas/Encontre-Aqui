# Encontre Aqui Api

## Projeto desenvolvido como Trabalho de Conclusão de Curso na Universidade Candido Mendes (UCAM) em 2021
 
![image](https://user-images.githubusercontent.com/72840768/221002569-edba52f7-fd51-403a-a739-eb54b366c7f2.png)



Projeto final apresentado ao Instituto de Formação Profissional Avançada da Universidade Cândido Mendes como exigência da disciplina de Trabalho de Conclusão de Curso, sendo requisito para a conclusão do curso Superior de Tecnologia em Análise e Desenvolvimento de Sistemas.

Orientadora: Profa. Ma. Rosana Fernandes Osório


## Introdução

### 1.1.	Descrição do Tema
O sistema “Encontre aqui” possui como equipe de desenvolvimento os alunos Andrey Lucas Vieira Costa, Gabriel Molina da Silva, Luiz Guilherme de Souza Ogeda e Rayssa Gomes Moreira, da Instituição Cândido Mendes. Este sistema foi desenvolvido para o trabalho de conclusão do curso de Análise e Desenvolvimento de Sistemas, com orientação realizada pela professora Rosana Osório.

O Encontre aqui tem como objetivo possibilitar que órgãos interessados, tipo: instituições de ensino, metrôs, barcas, shoppings e outros implantem o sistema para que usuários que perderam seus pertences de pequeno valor como documentos, casacos, mochilas, óculos e etc, possam localizá-las. Permitindo a busca de seus pertences a partir do local em que o objeto foi perdido.
	
### 1.2.	Justificativa
Todos os dias pessoas no Brasil estão cumprindo suas rotinas e afazeres circulando em caminhos que envolvem seu trabalho, estudo e lazer. Com isso, acabam perdendo seus pertences ou esquecendo em estabelecimentos, podendo existir dificuldade em identificar o local exato que possa ter esquecido ou perdido. De acordo com a divulgação da CTPM (Companhia Paulista de Trens Metropolitanos) em 2019 foram esquecidos 91.668 itens nas estações e interior dos trens. Dentre os itens esquecidos, 71% eram documentos. Perdas como essas podem tornar complexo muitos processos comuns na nossa sociedade.
Várias instituições fazem o trabalho de guarda de pertences de uma maneira descentralizada (correios, shoppings, lojas e etc..) e, muitas vezes, não divulgada para o público, o que acaba dificultando ainda mais.
Devido a isto e com objetivo de contribuir para solução desse problema, foi desenvolvido um sistema para conseguir consolidar e tornar público objetos que foram perdidos em determinados órgãos e outros estabelecimentos para que pessoas que perderam possam ter a oportunidade de rever o objeto perdido. 
Com a utilização do “Encontre aqui” será possível evitar que pessoas não consigam reaver seus pertences, evitar processos de retirada de segunda via de documentos, custos ligados a compra de novos bens e mitigar qualquer custo não mensurável que possam permear essas situações. 
### 1.3.	Objetivo Geral
O Encontre aqui é uma ferramenta que visa possibilitar de maneira fácil e colaborativa a localização de pertences perdidos nos órgãos interessados em oferecer esse serviço.

## 2.	CAPÍTULO – Modelo de Caso de Uso

### Diagrama de Caso de Uso 
![image](https://user-images.githubusercontent.com/72840768/221003351-d88a81a8-2ecf-4677-b433-1759084112a6.png)

### 2.1.	Descrição Textuais dos Atores
### 2.1.1.	 Cliente que perdeu o objeto
O cliente que perdeu o objeto será responsável por pesquisar o objeto perdido no site, preenchendo os parâmetros de pesquisa obrigatórios para efetivação da pesquisa e deverá sinalizar quando encontrar o objeto.



### 2.1.2.	 Cliente que encontrou o objeto
O cliente que encontrou o objeto será responsável por se cadastrar no site preenchendo os dados obrigatórios para efetivação do cadastro, por cadastrar as informações no site que correspondem ao objeto perdido, por comunicar o ponto de entrega do objeto perdido e notificar o ponto de referência do objeto encontrado.

	

### 2.1.3.	Administrador
O ADM será responsável por manter os pontos de entrega, os objetos e seus respectivos tipos, disponibilizar as informações estatísticas dos objetos para geração de dados informativos no sistema e manter os orgãos interessados cadastrados no sistema.

### 2.1.4.	Órgão interessado
Os Órgãos interessado serão responsáveis por se cadastrarem no site preenchendo os dados obrigatórios para efetivação do cadastro, por cadastrar as informações no site que correspondem aos objetos encontrados em seu estabelecimento, por validar os objetos encontrados cadastrados no site e informar o ponto de Referência onde o objeto foi encontrado.










### 2.2.	Descrições textuais dos casos de uso
### 2.2.1.	Encontrar objeto perdido:
●	Descrição: 
Este caso de uso está relacionado ao ator que perdeu um objeto e irá pesquisar no sistema se esse objeto foi encontrado e anunciado por algum usuário.

●	Atores envolvidos: 
- Cliente perdeu objeto 
- Sistema

●	Pré-condições: 
O usuário deverá preencher os campos obrigatórios do sistema para efetuar a busca.

●	Fluxo de Eventos: 
1.	FB – Fluxo Básico – Pesquisar objeto perdido
1.1.	O cliente acessa ao Sistema 
1.2.	O cliente informa no campo de pesquisa o objeto perdido e o ponto de referência e clica em pesquisar
1.3.	O sistema apresenta a lista de objetos perdidos
1.4.	O cliente verifica se algum item da lista é o objeto perdido
1.5.	O cliente encontra o objeto perdido
1.6.	O cliente que perdeu o objeto avisa que o objeto perdido foi encontrado [Estender o caso de uso Avisar que objeto perdido foi encontrado pelo cliente que perdeu] 
1.7.	E o caso de uso será encerrado	

2.2.2.	Cadastrar objeto encontrado
●	Descrição: 
Este caso de uso está relacionado ao ator que encontrou o objeto e irá anunciar no sistema, de forma que, qualquer usuário possa encontrar seu objeto perdido.


●	Atores envolvidos: 
- Cliente encontrou objeto
- Sistema

●	Pré-condições: 
O usuário deverá estar cadastrado no sistema para realizar o anúncio. 

●	Fluxo de Eventos:
FB – Fluxo Básico – Informar objeto encontrado:
1.	O cliente acessa o sistema através de login e senha
2.	O cliente aciona o botão de “Cadastrar objeto encontrado”
3.	O cliente preenche o cadastro do objeto encontrado, com os campos obrigatórios: Nome de objeto, descrição, tipo de objeto, ponto de referência e fotos. 
4.	O cliente aciona o botão “salvar objeto encontrado” 
5.	O sistema irá notificar o cliente que perdeu o objeto que o item foi encontrado [Estender o caso de uso Avisar que objeto perdido foi encontrado] (RN004) 
6.	O sistema irá informar o local que o objeto foi encontrado [Incluir caso de uso informar local que objeto foi encontrado]
7.	O sistema irá informar o ponto de entrega do objeto  (RN003)
8.	E o caso de uso será encerrado.


## 3.	CAPÍTULO – Modelo de Negócios
![image](https://user-images.githubusercontent.com/72840768/221004021-0e8d4175-9e91-4389-96fa-fa057f0f86ba.png)

##4.	CAPÍTULO - ARQUITETURA 

###4.1. – Descrição das tecnologias
	Inicialmente o Encontre Aqui será desenvolvido somente web, o backend do projeto será desenvolvido em PHP, com banco de dados MySQL, para o frontend usaremos HTML5, CSS e Javascript. Serão também utilizados o framework Bootstrap(CSS) e a biblioteca Jquery(Javascript).

###4.1.1. – Arquitetura das tecnologias

![image](https://user-images.githubusercontent.com/72840768/221004180-34e099d6-1358-4d69-b536-8619c9bb6427.png)

### 4.2 – Diagrama de Classe Conceitual 
![image](https://user-images.githubusercontent.com/72840768/221004280-e68fc892-577e-4e7f-9dbf-55f494bf7103.png)

## 5.	CAPÍTULO -  MODELO DE INTERAÇÕES 

  ### 5.1 Diagrama de Atividades – Cadastrar Objeto Encontrado
  ![image](https://user-images.githubusercontent.com/72840768/221004405-5b8c6799-315e-4a8c-aef4-f09f4e6b4099.png)

### 5.2 Diagrama de Atividades – Informar Objeto Perdido
![image](https://user-images.githubusercontent.com/72840768/221004491-ce50b268-9070-4045-b1fc-28e3a2a90469.png)


##6.	Projeto de Interface Gráfica

Hierarquia das Telas – Web
Neste item serão apresentadas as principais telas do sistema.
![image](https://user-images.githubusercontent.com/72840768/221004688-950e8360-2703-42d4-9ac2-bcdf44f1145d.png)

![image](https://user-images.githubusercontent.com/72840768/221004748-e1ec688d-e5ae-4eb2-87c6-570abd9adebf.png)
![image](https://user-images.githubusercontent.com/72840768/221004778-0bbc469f-2662-41a4-9cea-45f9d097777a.png)
![image](https://user-images.githubusercontent.com/72840768/221004818-74075774-c617-4890-8387-6cf1d3a4c1ba.png)
![image](https://user-images.githubusercontent.com/72840768/221004842-0bb5a615-8578-4a98-b018-f5da91663d4a.png)
![image](https://user-images.githubusercontent.com/72840768/221004865-a488d124-db89-490c-bf6a-1c2f8a4ad991.png)
![image](https://user-images.githubusercontent.com/72840768/221004905-0d55d928-80fb-46c2-b604-1316626cfccc.png)

### 6.1  Mapa de Navegação
![image](https://user-images.githubusercontent.com/72840768/221005006-7884785f-4f9f-48da-9ed3-35e144f11046.png)


###6.2  Descrição e Modelo dos Relatórios
Será disponibilizado no sistema painéis para acompanhamento do administrador e indicadores para verificação de métricas do negócio. O relatório contém as informações de objetos que mais se perderam por bairro, ponto de referência e por período; e objetos que foram encontrados por período.
Relatórios de objetos: O relatório poderá ser visualizado pelo administrador possibilitando acompanhar dados relativos aos objetos que foram encontrados, como: Status, sub status, o cliente que perdeu, o cliente que encontrou, o tipo de objeto perdido, o local de referência, as atualizações e a data. 



## 7.	Conclusão e trabalhos futuros
De acordo com o objetivo informado no início do projeto de atender uma necessidade da sociedade para facilitar a busca de objetos perdidos. 
O grupo realizou a especificação da solução do sistema com as seguintes funcionalidades: o sistema ENCONTRE AQUI com as seguintes funcionalidades: Cadastro de objetos encontrados, Localização e identificação de objetos perdidos, Informar que objeto perdido foi encontrado, Cadastro de usuários, Cadastro de pontos de entrega e geração de relatório contendo as informações de objetos que mais se perderam por bairro, local de retirada e por período; e objetos que foram encontrados por período.

O grupo encontrou dificuldades em mapear a solução de um problema em uma especificação utilizando os diagramas da UML (Ex.: Diagrama de atividades representando o modelo de negócio)

Será estudado para o Projeto Integrador II, a possibilidade de alterar o projeto de arquitetura para ser implementado em mobile.


