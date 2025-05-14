# TesteAPI

Este projeto contém testes automatizados da API desenvolvidos com o Postman e executados com o Newman localmente e via GitHub Actions (CI/CD).

Ferramentas utilizados para executar o projeto localmente:

Postman - Para requisição dos métodos GET, POST, PUT e DELETE. Criação de Collections e Ambientes 
VS Code - Necessário para criar um documento em yml e subir para workflow do github 
Newman - para executar coleções do Postman
Node.js - Executar código JavaScript fora do navegador e executar automações e scripts

Arquivos utilizados:

Auth.postman_collection.json
Users.postman_collection.json
Ambiente API.postman_environment.json
package.json
newman-tests.yml

ETAPAS DO PROJETO

Desenvolvimento dos métodos no Postman: Foi criado os seguintes métodos através da base URL https://serverest.dev

POST - Criar usuário
GET - Listar todos os usuário
GET - Buscar usuário por ID
PUT - Atualizar usuário
DELETE - Excluir usuário
POST - Login para obter token

Foi criado um ambiente para armazenar as seguintes váriaveis:
userId
base_url
email_unico

No campo "Script" de cada método foi desenvolvido os paramêtros para validação dos testes, utilizando a linguagem JavaScript. 

As Collections e Ambiente foram exportados para a pasta local do projeto. 

Foi criado arquivo newman-tests.yml para utilização na Pipeline Actions do GitHub

Após finalização do projeto local, foi realizado o versionamento do Projeto para o GitHub 

Lógica de Programação Utilizada
Variáveis dinâmicas: Para usar o mesmo ID em PUT, GET e DELETE.
Uso de pm.expect para validar tipo de resposta, status e dados obrigatórios.


