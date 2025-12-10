# Sistema de Gerenciamento de Venda de Ingressos e Sessões de Cinema

O objetivo do projeto é modelar um banco de dados para o gerenciamento da venda de ingressos e a programação das sessões de um cinema. Suas funcionalidades são:
● Cadastrar filmes e clientes;
● Gerenciar sessões e ingressos;
● Controlar assentos;
● Registrar as compras;
O banco de dados não deve permitir que o mesmo assento seja vendido em dois ingressos diferentes para uma mesma sessão ou que duas sessões ocorram na mesma sala e horário.
As entidades identificadas são filme, sessão, cliente, ingresso, sala, poltrona, compra e pagamento, as quais se relacionam da seguinte maneira:
● Um filme pode ser exibido em várias sessões. Um sessão exibe um filme.
● Uma sessão é hospedada em uma sala. Uma sala pode hospedar várias sessões.
● Uma sala contém várias poltronas. Uma poltrona é contida em uma sala.
● Uma sessão possui vários ingressos. Um ingresso pertence a uma sessão.
● Um ingresso reserva uma poltrona. Uma poltrona pode ser reservada por vários ingressos, porém apenas um por sessão.
● Uma compra adquire vários ingressos. Um ingresso é adquirido por uma compra.
● Um cliente pode realizar várias compras. Uma compra é realizada por apenas um cliente.
● Cada compra pode possuir múltiplos pagamentos. Um pagamento é referente a uma única compra.
● Cada ingresso é classificado por um tipo. Um tipo de ingresso classifica vários ingressos.

Modelo Conceitual, o qual identifica as entidades e seus atributos, foi realizado utilizando-se o software BrModelo. 
O Diagrama de Entidade-Relacionamento, concluído por meio do software Oracle Data Modeler, é responsável por identificar a cardinalidade e opcionalidade dos relacionamentos entre as entidades. 
Por fim, o Modelo Físico é representado mediante script Data Definition Language, o qual define as estruturas das tabelas e as suas constraints. Além disso, estão incluídos script DML para inserção de dados e script de consultas SQL nos dados das tabelas. 
