install dotnet 8

install mysql

update connecttion string in Startup.cs

dotnet tool install --global dotnet-aspnet-codegenerator

dotnet add package Microsoft.EntityFrameworkCore.Tools

# auto generate code
dotnet aspnet-codegenerator controller -name EmployeeController -m Employee -dc ApplicationDbContext --relativeFolderPath Controllers --useDefaultLayout --referenceScriptLibraries

# Run migration in database

dotnet ef migrations add InitialCreate
dotnet ef database update

# How to run application: 

dotnet dev-certs https --trust

dotnet run

