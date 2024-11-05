dotnet tool install --global dotnet-aspnet-codegenerator

dotnet add package Microsoft.EntityFrameworkCore.Tools

# auto generate code
dotnet aspnet-codegenerator controller -name EmployeeController -m Employee -dc ApplicationDbContext --relativeFolderPath Controllers --useDefaultLayout --referenceScriptLibraries

# How to run application: 

dotnet dev-certs https --trust

dotnet run

# Run migration in database

dotnet ef migrations add InitialCreate
dotnet ef database update











Mysql@localhost:3306
root
123123123