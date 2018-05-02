# basic-lambda-function

Setup
https://docs.aws.amazon.com/lambda/latest/dg/lambda-dotnet-coreclr-deployment-package.html

Install aws templates - dotnet new -i Amazon.Lambda.Templates::*
basic-lambda matthewbrett$ dotnet new lambda.EmptyFunction --name MyFunction --profile lambda-service --region ap-southeast-2
dotnet restore MyFunction.Tests/MyFunction.Tests.csproj
dotnet lambda deploy-function MyFunction --function-role lamdba-service-role
dotnet lambda invoke-function MyFunction --payload 'Some nonsense'

