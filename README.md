https://dotnet.microsoft.com/pt-br/download
C# Dev Kit
https://git-scm.com/downloads/wingi

dotnet new list
dotnet new sln -o Financeiro
dotnet new classlib -o Domain
dotnet sln add ./src/Domain/Domain.csproj

dotnet new xunit -o ./tests/Domain.Tests  
dotnet sln add ./tests/Domain.Tests/Domain.Tests.csproj

dotnet add package xunit

dotnet add reference ../../src/Domain/Domain.csproj


git init
git add .
git commit -m "initial"
