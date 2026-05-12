# avaliacao_01_algoritmos
Primeira Avaliação do caixeta

Aluno: João Victor Costa Souza /
Curso: 2608 - informatica para Internet

## Descrição Geral:

Opção 1 – Cadastrar funcionário: solicita nome, cargo, salário e data de admissão, armazenando os dados na matriz. O maximo é 10 funcionarios

Opção 2: solicita um nome, realiza a busca na matriz e exibe nome e cargo do funcionário encontrado. Caso não encontre, exibe "Nenhum resultado para a pesquisa".

Opção 3 – Exibir todos: lista todos os funcionários cadastrados em formato de tabela com nome, cargo, salário e data de admissão. Caso não haja nenhum cadastrado, informa essa situação.

Opção 4 – Sair: encerra o programa.



## Explicação das Decisões Aplicadas no Algoritmo:

4 vetores: cada linha representa um funcionário e cada coluna representa uma informação (nome, cargo, salário, data de admissão). Todos os campos são do tipo Caractere para simplificar o armazenamento na matriz.

Variável (total): controla quantos funcionários foram cadastrados, evitando ultrapassar o limite de 10 e garantindo que a pesquisa e listagem leiam apenas posições preenchidas.

Estrutura (Repita...Ate): mantém o menu em loop até o usuário escolher a opção 4.

Variável (encontrado): flag lógica usada na pesquisa para identificar se algum resultado foi localizado e exibir a mensagem correta ao final.
