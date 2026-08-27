# ExpenseLedger V2 Architecture Map

## Clean Architecture Layers

- Domain
- Application (CQRS + MediatR)
- Infrastructure (Redis, Logging, External Services)
- Persistence (EF Core + SQL Server)
- API (.NET 10)
- Blazor Server
- .NET MAUI Android

## Dependency Rules

- Domain -> None
- Application -> Domain
- Infrastructure -> Application + Domain
- Persistence -> Application + Domain
- API -> Application
- Blazor -> Contracts/API only
