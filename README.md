# Sistema de Gerenciamento de Venda de Ingressos e Sessões de Cinema

## Descrição do Projeto
Este projeto tem como objetivo modelar e implementar um banco de dados para gerenciamento de venda de ingressos e programação de sessões de cinema. Ele permite o controle completo de filmes, clientes, sessões, assentos, ingressos e compras, garantindo que não ocorram conflitos de reservas ou horários.

---

## Funcionalidades
O sistema oferece as seguintes funcionalidades:  
- Cadastro de filmes e clientes  
- Gerenciamento de sessões e ingressos  
- Controle de assentos  
- Registro de compras e pagamentos  

**Regras de negócio importantes:**  
- Um mesmo assento não pode ser vendido para dois ingressos diferentes na mesma sessão  
- Duas sessões não podem ocorrer na mesma sala e horário  

---

## Entidades e Relacionamentos
As principais entidades do sistema são: `Filme`, `Sessão`, `Cliente`, `Ingresso`, `Sala`, `Poltrona`, `Compra` e `Pagamento`.  

Relações entre as entidades:  
● Um filme pode ser exibido em várias sessões. Um sessão exibe um filme.
● Uma sessão é hospedada em uma sala. Uma sala pode hospedar várias sessões.
● Uma sala contém várias poltronas. Uma poltrona é contida em uma sala.
● Uma sessão possui vários ingressos. Um ingresso pertence a uma sessão.
● Um ingresso reserva uma poltrona. Uma poltrona pode ser reservada por vários ingressos, porém apenas um por sessão.
● Uma compra adquire vários ingressos. Um ingresso é adquirido por uma compra.
● Um cliente pode realizar várias compras. Uma compra é realizada por apenas um cliente.
● Cada compra pode possuir múltiplos pagamentos. Um pagamento é referente a uma única compra.
● Cada ingresso é classificado por um tipo. Um tipo de ingresso classifica vários ingressos.

---

## Modelagem do Banco de Dados

1. **Modelo Conceitual**  
   - Identifica as entidades e seus atributos;  
   - Desenvolvido usando o software BrModelo;

2. **Diagrama Entidade-Relacionamento (DER)**  
   - Identifica a cardinalidade e opcionalidade dos relacionamentos  
   - Desenvolvido com Oracle Data Modeler

3. **Modelo Físico**  
   - Representado por scripts **DDL (Data Definition Language)**, definindo tabelas e constraints  
   - Inclui scripts **DML** para inserção de dados  
   - Contém scripts de consultas SQL para manipulação e visualização de dados  

