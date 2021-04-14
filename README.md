# NN note

|| [**How to run**](#how-to-run) - [**TodoApi**](#TodoApi)  ||

## How to run

1. Clone this repository
2. Run from Visual Studio (Choose startup project)
   
## TodoApi
* Tutorial: Create a web API with ASP.NET Core 
    * Docs > .NET > ASP.NET Core > Tutorials > Web API apps > Create a web API
    * https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api
* database, in memory. In Startup.cs
```C#
services.AddDbContext<TodoContext>(opt => opt.UseInMemoryDatabase("TodoList"));
```
* list of endpoints
    * API	Description	Request body	Response body
    * GET /api/TodoItems	Get all to-do items	None	Array of to-do items
    * GET /api/TodoItems/{id}	Get an item by ID	None	To-do item
    * POST /api/TodoItems	Add a new item	To-do item	To-do item
    * PUT /api/TodoItems/{id}	Update an existing item  	To-do item	None
    * DELETE /api/TodoItems/{id}    Delete an item    	None	None

## MvcMovie
* Get started with ASP.NET Core MVC
* Docs > .NET > ASP.NET Core > Tutorials > Web apps > MVC > Get started
* https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/start-mvc
* list of endpoints
    * https://localhost:{PORT}/HelloWorld/Welcome
    * https://localhost:{PORT}/HelloWorld/Welcome/3?name=Rick
    * http://localhost:21061/HelloWorld/Welcome?name=Rick&numtimes=4
* 