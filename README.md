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

dotnet test

dotnet add reference ../../src/Domain/Domain.csproj

echo "# financeiro" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/RicardoBastos/financeiro.git

git push -u origin main