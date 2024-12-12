Projeto Conceitual: Sistema de Oficina Mecânica

Este repositório contém o esquema de banco de dados de um desafio proposto pela DIO.me,com a descrição do projeto conceitual para um sistema de gerenciamento de ordens de serviço em uma oficina mecânica. O objetivo é oferecer uma solução eficiente para organizar e controlar clientes, veículos, ordens de serviço, serviços realizados, peças utilizadas e equipes de trabalho.

Contexto do Projeto

Narrativa do Cliente
- Clientes levam veículos à oficina para consertos ou revisões periódicas.
- Cada cliente pode possuir um ou mais veículos.
- O cliente é identificado por informações como nome, CPF e contato.

Narrativa do Veículo
- Cada veículo possui informações como placa, modelo, marca, ano de fabricação e tipo (ex.: Carro, Moto, Caminhão).
- Um veículo está sempre associado a um cliente.

Narrativa da Ordem de Serviço (OS)
- As ordens de serviço (OS) são criadas para registrar os trabalhos realizados em um veículo.
- Cada OS inclui informações como número, data de emissão, valor total, status (ex.: Pendente, em execução, Concluída) e data prevista para conclusão.
- A OS é associada a um veículo e a uma equipe responsável pela execução.

Narrativa da Equipe
- As equipes são formadas por mecânicos especializados.
- Cada equipe é identificada por um nome único e é responsável pela execução de uma OS.

Narrativa do Serviço
- Um serviço representa um trabalho específico realizado em uma OS, como "Troca de óleo" ou "Alinhamento".
- Cada serviço possui uma descrição e um valor de mão de obra.
- Uma OS pode incluir múltiplos serviços, e um serviço pode ser executado em várias OS.

Narrativa da Peça
- Peças utilizadas nos serviços são registradas com informações como nome, descrição e valor unitário.
- Uma OS pode incluir várias peças, e uma peça pode ser utilizada em diferentes OS.

Tabelas Associativas
- ServiçoOrdemServico: Relaciona serviços a ordens de serviço, indicando quais serviços foram executados em cada OS.
- PecaOrdemServico: Relaciona peças a ordens de serviço, indicando quais peças foram utilizadas em cada OS e suas quantidades.

Consultas Permitidas
Com base no modelo, o sistema permite realizar as seguintes consultas:

1. Listar os veículos associados a um cliente específico.
2. Consultar todas as ordens de serviço de um veículo.
3. Identificar o status atual de uma OS (ex.: Pendente, em execução, Concluída).
4. Obter o valor total de uma OS, incluindo serviços e peças.
5. Listar os serviços mais realizados e as peças mais utilizadas na oficina.
6. Consultar os mecânicos de uma equipe específica.
7. Monitorar as ordens de serviço pendentes ou em execução.

Conclusão
Este modelo conceitual foi projetado para atender às necessidades operacionais de uma oficina mecânica, garantindo a organização de dados essenciais e facilitando a consulta e análise de informações. Ele oferece flexibilidade para expansões futuras e eficiência no gerenciamento de ordens de serviço.
