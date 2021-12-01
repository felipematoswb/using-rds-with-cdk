# Welcome CDK TypeScript project!

This is a blank project for TypeScript development with CDK.

## To execute this project

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
[AWSCLi](https://aws.amazon.com/pt/cli/), [Git](https://git-scm.com), [Node.js](https://nodejs.org/en/). 
Além disto é bom ter um editor para trabalhar com o código como [VSCode](https://code.visualstudio.com/).


```bash
# Clone este repositório
$ git clone <https://github.com/felipematoswb/using-rds-with-cdk.git>

# Acesse a pasta do projeto no terminal/cmd
$ cd using-rds-with-cdk

# Configure suas credenciais
$ aws configure

# Instale as dependências
$ npm install

# Execute a aplicação em modo de desenvolvimento
$ cdk deploy

# Acesse a console da AWS e verifique os serviços EC2 e RDS estão configurados.
```

### Teste a conexão entre a EC2 e o RDS.

```bash
# Acesse o serviço EC2
# Clique na instancia configurada
# Clique em Conectar
# Utilize o menu Session Manager e clique em Executar
# Irá abrir a console da instancia
# Atualize os pacotes
$ sudo yum update -y

# Instale o postgres
$ sudo yum install postgresql postgresql-server -y

# Acesse Secret Manager e Retrive passwork
# Conecte no banco
$ psql -p 5432 -U postgres -h YOUR_DB_ENDPOINT
```

## Useful links
* https://constructs.dev/packages/@aws-cdk/aws-rds/v/1.134.0
* https://constructs.dev/packages/@aws-cdk/aws-ec2/v/1.134.0
* https://constructs.dev/packages/@aws-cdk/aws-iam/v/1.134.0


## Useful commands

 * `npm run build`   compile typescript to js
 * `npm run watch`   watch for changes and compile
 * `npm run test`    perform the jest unit tests
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template
