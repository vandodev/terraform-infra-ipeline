<h3 align="center">
  Pipeline de Infraestrutura (AWS + Terraform + Github Actions + Multi Env)
</h3>

<p align="center">
  <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-%2304D361">
  <img alt="Version: 1.0" src="https://img.shields.io/badge/version-1.0-yellowgreen">
</p>

<p align="center" width="100%">
    <img width="100%" src="https://github.com/user-attachments/assets/f21bbb7f-584c-4823-a484-199c3dd1b336"> 
</p>

<p align="center" width="100%">
    <img width="100%" src="https://github.com/user-attachments/assets/d6819daa-4c37-4d81-8ba8-27f86b76a54d"> 
</p>

### Fista de tarefas

Setup do projeto
- [x] Criar repositório da pipeline de infra no Github
- [x] Criar bucket s3 (dev e prod)
- [x] Escrever código terraform que criará recurso na AWS

Configurar conta AWS
- [x] Configurar AWS IAM 
- [ ] Configurar tTrust Relationship via OpenID
- [x] Criar role
- [x] Criar bucket s3 para armazenar os Stalefiles do terraform
- [x] Criar a tabela no DynameDB para realizar o look para modificações concorrentes

Criar o Reusable Workflow de Terraform
- [x] Configurar os inputs do workflow 
  - [x] env 
  - [x] aws assume role arn 
  - [x] aws region 
  - [x] aws s3 bucket statefile 
<<<<<<< HEAD
  - [x] aws dynamodb table lock  
- [x] Criar uma branch develop
=======
  - [x] aws dynamodb table lock 
>>>>>>> develop

Configurar o setup do workflow  
- [x] Clonar o repositório 
- [x] Configurar a AWS CLI 
- [x] Configurar o Terraform CLI 

- [x] Configurar o step Terraform Init 
- [x] Configurar o step Terraform Validate 
- [x] Configurar o step do Terraform Plan 
- [x] Configurar o step do Terraform Apply

Configurando a pipeline para o ambiente de DEV: 
- [x] Configurar o reusable workflow do Terraform (develop) 
- [x] Realizar a criação de um bucket S3 no ambiente de DEV 

Configurando a pipeline para o ambiente de PROD: 
- [x] Configurar o reusable workflow do Terraform (main) 
- [x] Realizar a criação de um bucket S3 no ambiente de PROD 

Configurar o suporte para Terraform Destroy 
- [x] Configurar o step de ler destroy_config.json 
- [x] Configurar o step do Terraform Destroy 
- [x] Ajustar os steps de plan e apply para considerar o destroy 
- [x] Realizar o destroy no ambiente de Prod 
- [ ] Realizar o destroy no ambiente de Dev 





