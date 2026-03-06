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
