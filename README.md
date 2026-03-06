# DESAFIO-QA-BEEDOO-2026
Qual você acredita ser o objetivo da aplicação?
A aplicação aparenta ter como objetivo realizar o gerenciamento de cursos, permitindo que usuários cadastrem novos curis e visualizem os cursos já cadastrados no sistema. Trata-se de uma interface simples que possibilita o controle e a organização de informações relacionadas aos cursos disponíveis.
Quais são os principais fluxos disponíveis?
Bom, consegui identificar dois fluxos principais dentro da aplicação:
- Listagem de cursos: Que permite o usuário de visualizar todos os cursos cadastrados no sistema através da tela "Lista de cursos".
- Cadastro de curso: Que permite ao usuário de adicionar um novo curso ao sistema por meio da opção "Cadastrar curso", preenchendo um formulário com informações relevantes sobre o curso.
Quais pontos do sistema você considera mais críticos para teste?
- Validação do formulário de cadastro: garantir que campos obrigatórios sejam preenchidos corretamente e que o sistema trate entradas inválidas de forma adequada.
- Persistência dos dados: verifcar se os cursos cadastrados são armazenados corretamente e exibidos na lista após o cadastro ou após atualização da página.
- Exibição da lista de cursos: testar cenários como lista vazia, grande quantidade de cursos e possíveis duplicidades.
- Navegação entre telas: garantir que os botões de navegação, como "Listar cursos" e "Cadastrar curso", direcionem corretamente para as respectivas páginas sem erros.
- Tratamento de erros e feedbacks ao usuário: validar se o sistema apresenta mensagens claras em caso de falhas ou dados inválidos.
  
## Casos de teste
Os cenários e casos de teste foram documentados na planilha abaixo:
https://docs.google.com/spreadsheets/d/1P9_lkNOPuWbMjK42TXWorNKrJoyIAbaW5w8OEOmr0BI/edit?usp=sharing

## Evidências de Teste
As evidências e capturas de tela dos testes realizados estão disponíveis no documento abaixo:
https://docs.google.com/document/d/1d69LxZEFJiyPBe1QM4oA0QSbLrcaIS2F/edit?usp=sharing&ouid=107109538030229279579&rtpof=true&sd=true

## Registro de Bugs
Durante os testes foram identificados os seguintes problemas:

### Bug01 - Cadastro permite envio com campos vazios
Título: Cadastro de curso permite salvar sem preencher campos obrigatórios 
Passos para reproduzir: 
1. Acessar a página Cadastrar curso
2. Deixar os campos vazios
3. Clicar em Salvar
Resultado atual: O sistema permite salvar o curso mesmo sem preencher os campos.
Resultado esperado: O sistema deveria bloquear o cadastro e exibir uma mensagem informando que os campos são obrigatórios.
Severidade: Alta

### Bug02 - Falta de mensagem quando a lista está vazia
Título: Sistema não exibe mensagem quando não existem cursos cadastrados.
Passos para reproduzir: 
1. Acessar Listar cursos
2. Não ter cursos cadastrados
Resultado atual: A tela aparece vazia sem nenhuma informação.
Resultado esperado: O sistema deveria mostrar uma mensagem como "Nenhum curso cadastrado"
Severidade: Baixa
