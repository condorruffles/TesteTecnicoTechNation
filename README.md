# Descri��o

Este projeto � um teste t�cnico desenvolvido, especialmente, para avaliar as suas
habilidades como desenvolvedor fullstack. Para isso, voc� deve usar no frontend HTML,
CSS, JS, jQuery, Bootstrap e biblioteca para cria��o de gr�ficos. E para o backend C# com a
vers�o LTS mais recente do .Net e SQL Server.
A proposta � a cria��o de uma tela do sistema financeiro de uma empresa com os
dados das notas fiscais emitidas no ano passado (2023) e um dashboard. Essa ferramenta
ser� utilizada pelo pessoal respons�vel pelo financeiro para manter o controle das notas e
saber os principais indicadores.

# Tecnologias utilizadas

- .NET 8.0
- SQL SERVER
- jQuery 3.7.1
- Razor
- Dapper ORM
- Docker
- HTML, CSS, JS

# Como iniciar

- Acessar o local no reposit�rio
- Utilizar o comando `docker-compose up -d`
- Conectar no SQL-SERVER criado pelo container utilizando a ConnectionString = `Server=localhost,1433;User ID=sa;Password=YourStrong@Passw0rd;Trusted_Connection=False;TrustServerCertificate=True;`
- Utilizar o script em `./SQL/unecontDB.sql` para cria��o e povoamento do banco `unecontDB`
- abrir o sistema: ele estar� hospedado por padr�o na porta  `https://localhost:3060`

# Considera��es importantes

- Pensando em um sistema escal�vel foi utilizado o Dapper ORM para mapeamento do banco de dados por ser mais perform�tico.
- As l�gicas de consultas mais complexas est�o armazenadas no banco em TVFs (Table-valued functions).
- A arquitetura do sistema foi desenvolvida visando os conceitos de CleanArchitecture, SOLID, DDD e CleanCode.
