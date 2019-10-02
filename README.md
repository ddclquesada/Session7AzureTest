# Web Services and Backend Course

## Contact
- Esteban Solano @stvansolano 
- Email: stvansolano@outlook.com 
- Blog: http://stvansolano.github.io/blog

## Installation & tooling

- [DotNet Core @2.2](https://dotnet.microsoft.com/download/dotnet-core/2.2)
- [VS 2019](https://visualstudio.microsoft.com/vs/)

VS Code extensions (Ctrl+Shift+P > Install Extensions):

### C# Extensions & Tooling

`dotnet tool install --global dotnet-aspnet-codegenerator --version 2.2.3`

### VS Code extensions
- C# Extensions
- C#
- C# Snippets
- C# FixFormat
- EditorConfig for VS Code

Chrome extensions
- [JSON Formatter](https://chrome.google.com/webstore/search/json)

## Links Session-01

## Session 01 - .NET Core Basics

.NET Core ~2.2 Commands

```
dotnet --info
dotnet new web
dotnet restore
dotnet build
dotnet run
```

-VS Code Configuration

```
dotnet watch run
```

## Links session 02 

- https://petstore.swagger.io/

- Postman - https://getpostman.com

- [Routing](https://docs.microsoft.com/en-us/aspnet/web-api/overview/web-api-routing-and-actions/attribute-routing-in-web-api-2#optional)

## Session 03 Links:

- [CORS](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS)

## Session 04 Links:
- [EntityFramework Core](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/#update-the-database)
- [JSON Patch](http://jsonpatch.com/)
- [EF Migrations](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/#update-the-database)

## Session 05 Links (Docker):
- [Docker](https://docs.docker.com/docker-for-windows/)

## Session 06 Links:

- [JWT](https://jwt.io/introduction/)
- [CosmosDB](https://docs.microsoft.com/en-us/azure/cosmos-db/introduction)

OData links:
- [OData 1](https://www.odata.org/getting-started/learning-odata-on-postman/)
- [OData 2](https://www.odata.org/getting-started/understand-odata-in-6-steps/)
- [GraphQL](https://developer.okta.com/blog/2019/04/16/graphql-api-with-aspnetcore)

GraphQL links:
[GraphQL 1](https://graphql.org/)

## Practice indications

### Practice 01

1) Create an HomeController MVC
2) Display a View (HTML) as default home page root (https://localhost:44357/)
3) Consume the `/products` endpoint

Commit + push to GitHub at: https://github.com/[your-user]/backend-services-course-cenfotec/tree/session-01/practice/practice-01

### Practice 02

1) Create a `CategoriesController` in the Web API
2) Add a `Get` endpoint
3) Add some Category records to database
4) Fetch Categories from database

Commit + push to GitHub at: https://github.com/[your-user]/backend-services-course-cenfotec/tree/session-04/practice/practice-02

### Practice 03

1) Create a new Azure account
2) Create a new GitHub repo with source code from branch `/session-07`. [Link](https://github.com/stvansolano/backend-services-course-cenfotec/tree/session-07/) **> Remember to commit + push to GitHub regularly.**

3) Create an Azure DevOps account and nickname (use your same nickname from GitHub)
4) Create a new AzureDevOps project (public) called MyAzureDevOpsLab

5) Create a new Pipeline from repo in step #2 with YAML editor and copy-paste the `/azure-pipelines.yml` contents from `session-07`

6) From Azure, create a new Azure Container Registry (again, use your nickname from GitHub for the ACR)

7) Build and push the `WebServer` image into your Azure Container Registry called `WebServer` with tag `latest`.

8) From Azure, try creating a new Container Instance from your image.

9) Do the same with WebClient by either changing the `azure-pipelines.xaml` or creating new pipelines accordingly.

10) Paste the following in a TXT file with your details and commit/push in your forked version of this project:

- Azure DevOps Repo URL
- Github Repository you used