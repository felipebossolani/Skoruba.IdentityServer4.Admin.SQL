# Projeto Skoruba.IdentityServer4.Admin com SQL

Projeto contém o necessário para subir uma aplicação baseada no excelente projeto [Skoruba.IdentityServer4](https://github.com/skoruba/IdentityServer4.Admin) com banco de dados em SQL. 
Projeto feito para estudos. **Não utiliza-lo em ambientes produtivos!!**

# Utilização do Repositório

Baixe o repo através do git clone:
```
git clone https://github.com/felipebossolani/Skoruba.IdentityServer4.Admin.SQL.git
```
E depois os seguintes comandos:
```
cd Skoruba.IdentityServer4.Admin.SQL.git
start Skoruba.IdentityServer4.Admin.SQL.sln
```

Os dados padrão de configuração são:
```
server = localhost
user = sa
pass = passworD@123
```

Caso queria utilizar uma imagem docker do SQL. Rode o seguinte comando:
```
docker run --name sql1 -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=passworD@123" -p 1433:1433 -v sqldata1:/var/opt/mssql -d mcr.microsoft.com/mssql/server:2017-latest
```

Você precisa executar os 3 projetos abaixo:
```
Skoruba.IdentityServer4.Admin
Skoruba.IdentityServer4.Admin.Api
Skoruba.IdentityServer4.STS.Identity
```

Os dados do admin são
```
user = admin
pass = Pa$$word123
```
