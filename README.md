# The application is backtofront practice

dotnet new --list

dotnet new webapi -o  apiGateways\OcelotApiGw
dotnet new webapi -o apiGateways\Shopping.Aggregator

dotnet new classlib -o buildBlocks\EventBus.Messages

dotnet new webapi -o services\Basket\Basket.API

dotnet new webapi -o services\Catalog\Catalog.API

dotnet new webapi -o services\Discount\Discount.API
dotnet new webapi -o services\Discount\Discount.Grpc

dotnet new webapi -o services\Ordering\Ordering.API
dotnet new classlib -o services\Ordering\Ordering.Application
dotnet new classlib -o services\Ordering\Ordering.Domain
dotnet new classlib -o services\Ordering\Ordering.Infrastructure

dotnet new web -o web\AspnetRunBasics



dotnet sln add apiGateways\OcelotApiGw
dotnet sln add apiGateways\Shopping.Aggregator
dotnet sln add buildBlocks\EventBus.Messages
dotnet sln add services\Basket\Basket.API
dotnet sln add services\Catalog\Catalog.API
dotnet sln add services\Discount\Discount.API
dotnet sln add services\Discount\Discount.Grpc
dotnet sln add services\Ordering\Ordering.API
dotnet sln add services\Ordering\Ordering.Application
dotnet sln add services\Ordering\Ordering.Domain
dotnet sln add services\Ordering\Ordering.Infrastructure
dotnet sln add web\AspnetRunBasics


