# Comandos iniciais:
``` bash
  mkdir aula-desafio21dias-mvc-entity-framework
  cd aula-desafio21dias-mvc-entity-framework
  dotnet new mvc
```

# Comandos git:
``` bash
  code .gitignore 
```
### gerei o conteúdo para ignorar como (Windows, Linux, Mac, DotnetCore, VisualStudioCore) no link: https://www.toptal.com/developers/gitignore
- Criei o repositório e rodei os comandos

``` bash
  git init
  git add .
  git commit -m "Iniciando projeto"
  git remote add origin git@github.com:didox/aula-desafio21dias-mvc-entity-framework.git
  git branch -M main
  git push -u origin main
```

# Componentes instalados:
``` bash
  dotnet add package Microsoft.EntityFrameworkCore --version 5.0.9
  dotnet add package Microsoft.EntityFrameworkCore.Tools --version 5.0.9
  dotnet add package Microsoft.EntityFrameworkCore.SqlServer --version 5.0.9
  dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design --version 5.0.2
```

# Comandos para migração:
``` bash
dotnet tool install --global dotnet-ef
dotnet ef migrations add CarroAdd
dotnet ef database update
```

# Instalação do code generator
``` bash
dotnet tool install -g dotnet-aspnet-codegenerator
```

# Gerando o scaffold de Carros
``` bash
dotnet aspnet-codegenerator controller -name CarrosController -m Carro -dc DbContexto --relativeFolderPath Controllers

dotnet aspnet-codegenerator controller -name MarcasController -m Marca -dc DbContexto --relativeFolderPath Controllers

```

