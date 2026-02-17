## Dotnet commands

#### Create New Solution File

A Solution file (.sln) is a master container that groups multiple related Projects (.csproj) into a single workspace. It doesn't hold code itself, it stores metadata and paths to coordinate how those projects build, interact, and depend on each other.

The name of the file will be based on the name of the folder it was created on.

```bash
  dotnet new sln
```

#### Create New Web-API Projet template

-n
-controllers: enable the option to make and separate into controllers

```bash
  dotnet new webapi -n {name} -controllers
```

#### Create New Class Lib Projet template

```bash
  dotnet new classlib -n {name}
```

#### Add a Project To The Solution File

```bash
  dotnet sln add {name}
```

#### run a C# project from the terminal

```bash
  dotnet run
```

#### run a C# project Hot reload enabled

It run with a file watcher, that may change the result in a active run without stop and run again

```bash
  dotnet watch
```

#### Create new migration

Use this Entity Framework Core (EF Core) command to generate a new database migration based on the current DbContext model.

- **InitialCreate** → Migration name
- **-p {project name}** → Project containing the `DbContext` and migrations
- **-s {startup project}** → Startup project used to load configuration (e.g., connection string, Where app runs and config exists)

```bash
  dotnet ef migrations add InitialCreate -p {project name} -s {startup project}
```

#### Remove Last Migration

Use this Entity Framework Core (EF Core) command to remove the most recently added migration.

- Removes the **last migration** if it has not been applied to the database
- **-p {project name}** → Project containing the `DbContext` and migrations
- **-s {startup project}** → Startup project used to load configuration (e.g., connection string, Where app runs and config exists)

```bash
dotnet ef migrations remove -p Persistence -s API
```

#### Build the Project

Use this command to compile the application and verify that the code builds successfully.

- Compiles the project and checks for errors
- Does **not** run the application
- Useful for validating changes before running or deploying

```bash
dotnet build
```

#### Update database

Use this Entity Framework Core (EF Core) command to apply pending migrations to the database. This updates the database schema to match the current data model.

- **-p {project name}** → Project containing the `DbContext` and migrations
- **-s {startup project}** → Startup project used to load configuration (e.g., connection string, Where app runs and config exists)

```bash
dotnet ef database update -p {project name} -s {startup project}
```

#### Drop database

Use this Entity Framework Core (EF Core) command to permanently delete the entire database. This removes both the schema and all stored data.

- **-p {project name}** → Project containing the `DbContext` and migrations
- **-s {startup project}** → Startup project used to load configuration (e.g., connection string, Where app runs and config exists)
- **-f (force)** → (Optional) Force the drop without asking for confirmation

```bash
dotnet ef database update -p {project name} -s {startup project}
```

## React commands

#### Get all items

```http
  GET /api/items
```

#### Get all items

```http
  GET /api/items
```

## Git commands

#### Get all items

```http
  GET /api/items
```

#### Get all items

```http
  GET /api/items
```
