Após acessar a conta AWS, você pode criar uma Função Lambda do zero ou usar o modelo template. 
A AWS Lambda é um serviço que possibilita executar códigos em resposta a eventos sem a necessidade de gerenciar sevidores. 
No caso do exemplo do desafio da Criação de um Assistente de Delivery, foi escolhida a função Lambda de encadeamento de prompts de IA com o Amazon Bedrock. 
Escolhida a função Lambda, é necessário implantar e executar a função para que se torne editável para as demais configurações. 
Implantada a função, será necessário configurar as permissões IAM e as permissões do modelo. 
Clicando em Editar, é possível alterar as configurações IAM em "Configurações"-> aba Permissões clicar em "Visualizar no IAM" -> "Adicionar permissões" e adicionar todas as permissões referentes ao Bedrock. 
Em seguida, em Design, é necessário selecionar todos os blocos de ações do Bedrock, é necessário selecionar o modelo disponível. No caso, foi usado o modelo Haiku Claude 3. 
Todas as configurações de permissões e modelos realizadas, será necessário montar o prompt e as variáveis de entrada para cada bloco de ação. 
No caso foram usadas 3 caixas. Então foram 3 solicitações: ideias de combinações de comidas, combinações de bebidas e lugar ideal, respectivamente. 
É ideal selecionar o total de tokens limites para cada bloco também. 
É importante salvar ao terminar as edições para executar sempre a versão mais atualizada. 
