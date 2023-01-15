# JDBC vs JPA

Depois de aprender um pouco sobre a linguagem #SQL conheci duas especificações essenciais quando vamos trabalhar com banco de dados relacional e persistência de objetos com a linguagem #java , o #JDBC e o #JPA. Por isso, visto tal importância, de uns dias para cá decidi estudar sobre essas tecnologias para tentar me aprofundar no tema. Neste post, falarei sobre o que aprendi até o momento.

Primeiramente vi que a função principal dessas tecnologias é conectar a aplicação Java com o banco de dados. Engraçado que quando eu estava estudando SQL me perguntava como funcionava esse processo, como as duas camadas eram conectas... Está aí a resposta, rs.

Continuando, aprendi que elas trabalham como uma camada intermediária, ficando entre a primeira camada (aplicação Java) e a terceira camada (banco de dados). O objetivo é facilitar e padronizar a comunicação entre as duas vertentes. Interpretar e converter os comandos para que os dados sejam manipulados.

Então me surgiu a seguinte dúvida: afinal, qual a diferença entre o JDBC e o JPA?

Em resumo, vi que as grandes diferenças estão na verbalidade do código e no acoplamento, além de alguns outros detalhes.

📌 Com o JDBC iremos precisar escrever os scripts para na mão. Já o JPA cuida disso para nós. Como consequência escrevemos códigos menos verbosos;

📌 O JDBC é altamente acoplado ao banco. Para cada tipo precisaremos escrever um script diferente para realizar a manipulação. Caso alterarmos o tipo de banco de dados da aplicação precisaremos modificar também diversas linhas de código, ou seja, mais trabalho. Já o JPA independe do tipo de banco de dados e o um mesmo código pode ser usado em vários tipos de bancos.

📌 Com o JPA, o desenvolvedor consegue fazer a aplicação OO sem ter que se preocupar com a linguagem do banco de dados, pois a própria especificação cuidará disso.

Enfim, aprendi que ambas as tecnologias são importantíssimas quando queremos integrar a nossa aplicação com o banco de dados, entretanto vi que utilizar o JPA torna o desenvolvimento mais rápido, porém é de extrema importância saber como tudo funciona debaixo dos panos.
