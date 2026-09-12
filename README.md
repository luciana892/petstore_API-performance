Teste de API REST — do manual à CI/CD

Repositório criado para o Projeto de Teste de API REST, com foco na execução de testes de forma manual e automatizada, utilizando Postman e Newman.

Tecnologias utilizadas
Postman Web
Node.js v18.16.1
Newman v5.3.2
newman-reporter-html
Documentação
Análise Técnica: Analise/
Documentação da API: Swagger — ServeRest
Como instalar o ambiente
1. Instalar o Node.js

Instale o Node.js em seu computador.

Baixar Node.js

2. Instalar o Newman

Realize a instalação do Newman de forma global:

npm install -g newman

Mais informações: Newman no npm

3. Instalar o Newman Reporter HTML

A instalação do newman-reporter-html é opcional e permite gerar relatórios HTML dos testes.

npm install -g newman-reporter-html

Mais informações: newman-reporter-html no npm

Como executar os testes
Pelo Postman Web ou Desktop
Importe a Collection.
Importe o Environment.
Execute os testes de forma manual ou automatizada.
Pelo Newman

Abra o console de sua preferência e execute o comando:

newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
Executando os testes com relatório HTML

Para executar os testes e gerar o relatório utilizando o htmlextra:

newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
Relatório

Ao executar os testes utilizando o reporter htmlextra, será gerado um arquivo HTML contendo os resultados da execução dos testes.

Esse relatório pode ser utilizado para consultar as validações realizadas durante a execução da coleção.

Report

Se você optou por rodar os testes com o report htmlextra,você gerou um arquivo html com o resultado dos testes e para verificar as validações voce pode abrir a pasta newman que foi criada no local em que os arquivos de collectione e environment se encontram.

Contato

E-mail: lucianavaleriana45@gmail.com

LinkedIn: linkedin.com/in/lucianavaleriana

Projeto — Teste de API REST do manual à CI/CD porem para testes de performance
