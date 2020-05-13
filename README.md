# Be.Vlaanderen.Basisregisters.Testing.Infrastructure [![Build Status](https://github.com/Informatievlaanderen/infrastructure-tests/workflows/CI/badge.svg)](https://github.com/Informatievlaanderen/infrastructure-tests/actions)

Contains unit-tests to validate your event types and assembly.
This is a source-only package, meaning that upon installation, it will create a file `InfrastructureEventsTests.cs` in your project directory.
Note that you might still have to update that file with the assembly containg your events under test.

## Usage

Add a dependency in the `paket.dependencies` file:

```csharp
nuget Be.Vlaanderen.Basisregisters.Testing.Infrastructure.Events ~> 1.0
```

Reference the dependency in the `paket.references` file of the project where you want to include the tests:

```csharp
Be.Vlaanderen.Basisregisters.Testing.Infrastructure.Events
```

Upon the next `paket install`, a file called `InfrastructureEventsTests.cs` will be added to your directory (you should commit this to your repository).
