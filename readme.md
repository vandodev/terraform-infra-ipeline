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
- [ ] Configurar os inputs do workflow 
  - [ ] env 
  - [ ] aws assume role arn 
  - [ ] aws region 
  - [ ] aws s3 bucket statefile 
  - [ ] aws dynamodb table lock 

Configurar o setup do workflow  
- [ ] Clonar o repositório 
- [ ] Configurar a AWS CLI 
- [ ] Configurar o Terraform CLI 

- [ ] Configurar o step Terraform Init 
- [ ] Configurar o step Terraform Validate 
- [ ] Configurar o step do Terraform Plan 
- [ ] Configurar o step do Terraform Apply

Configurando a pipeline para o ambiente de DEV: 
- [ ] Configurar o reusable workflow do Terraform (develop) 
- [ ] Realizar a criação de um bucket S3 no ambiente de DEV 

Configurando a pipeline para o ambiente de PROD: 
- [ ] Configurar o reusable workflow do Terraform (main) 
- [ ] Realizar a criação de um bucket S3 no ambiente de PROD 

Configurar o suporte para Terraform Destroy 
- [ ] Configurar o step de ler destroy_config.json 
- [ ] Configurar o step do Terraform Destroy 
- [ ] Ajustar os steps de plan e apply para considerar o destroy 
- [ ] Realizar o destroy no ambiente de DEV 
- [ ] Realizar o destroy no ambiente de R 





