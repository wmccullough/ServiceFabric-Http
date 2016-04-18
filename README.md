# Getting Started

**What is this?**
This project provides a set of libraries and framework components for enabling middleware communication with [Azure Service Fabric](https://azure.microsoft.com/en-us/documentation/services/service-fabric/). 

This project is built on [Asp.Net Core](http://docs.asp.net/en/latest/index.html)

Note: At this time, the project uses both stable and unstable builds of the dotnet cli. In order build, you may need to install versions of the dotnet cli. For more information on installing DNX, refer to the following website:

[DotNet CLI](https://github.com/dotnet/cli)

# Libraries for HTTP-based Azure Service Fabric services

This project contains three components:

##### C3.ServiceFabric.HttpCommunication
An implementation of `ICommunicationClient` (part of the Service Fabric SDK) for HTTP-based communication between Service Fabric services. 
It resolves services and contains retry logic. 
Please look at [HTTP Communication](https://github.com/c3-ls/ServiceFabric-Http/wiki/HTTP-Communication) for details.

##### C3.ServiceFabric.HttpServiceGateway
A HTTP-based gateway, implemented as an ASP.NET Core middleware. 
Please look at [HTTP Gateway](https://github.com/c3-ls/ServiceFabric-Http/wiki/HTTP-Gateway) for details.

##### C3.ServiceFabric.AspNetCore.StatelessHost
A hosting library for stateless ASP.NET Core-based Service Fabric services. 
With this library, it's not required to publish the app to your local Service Fabric cluster whenever you want to start/debug it locally. 
Instead, you can just 'dotnet run' or 'dotnet watch' your app! This is a huge time saver during development.
Please look at [Stateless ASP.NET Core Host](https://github.com/c3-ls/ServiceFabric-Http/wiki/Stateless-ASP.NET-Core-Host) for details.

You can find more documentation in our [Wiki](https://github.com/c3-ls/ServiceFabric-Http/wiki) 

[![Build status](https://ci.appveyor.com/api/projects/status/glormo3hm3wsdwm4/branch/master?svg=true)](https://ci.appveyor.com/project/cwe1ss/servicefabric-httpservicegateway/branch/master)

## Contributions

Feel free to post issues, questions and feedback as an issue in this repository. 
If you want to contribute code please make sure you discuss the change with us before
you send the pull request if it contains major or breaking changes.
