para crear el proyecto:

	  $ dotnet new sln --name EcommerceSolution

despues creamos el src

	  $ mkdir src
   
creamos las libs dentro de core (no es necesario incluirlas dentro de core)

	  $ dotnet new classlib -o src/Core/Ecommerce.Domain
	  $ dotnet new classlib -o src/Core/Ecommerce.Application

	  $ dotnet new classlib -o src/Infrastructure --name Ecomerce.Infrastrructure
   
la api hace las vezes de los controllers (la capa de framework)

	  $ dotnet new webapi -o src/Api --name Ecommerce.Api 
