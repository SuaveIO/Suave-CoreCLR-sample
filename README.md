# Sample Suave hello world using .NET Core

1. Install .NET Core SDK 1.0 sdk from http://dot.net
2. `dotnet restore`
3. `dotnet run`

by default it's avaiable at http://localhost:8083 

Use command line arguments to change ip/port

```
Usage:
    --ip ADDRESS   ip address (Default: 127.0.0.1)
    --port PORT    port (Default: 8083)
```

The dotnet version is `1.0.1`

## Build Status

| Platform                  | Status         |
| ------------------------- | -------------- |
| Windows                   | [![Build status](https://ci.appveyor.com/api/projects/status/qpwsi14ndxuv0gpl?svg=true)](https://ci.appveyor.com/project/AdemarGonzalez/suave-coreclr-sample) |
| Ubuntu 14.04 / OSX 10.11  | [![Build status](https://travis-ci.org/SuaveIO/Suave-CoreCLR-sample.svg?branch=master)](https://travis-ci.org/SuaveIO/Suave-CoreCLR-sample) |


### Win/Mac Osx 10.11/Ubuntu 14.04

1. `dotnet restore`
2. `dotnet run`

### Docker

To clone, build and run inside the `microsoft/dotnet:latest` docker container

1. `docker run -p 8083:8083 -it microsoft/dotnet:latest`
2. `git clone https://github.com/SuaveIO/Suave-CoreCLR-sample.git ~/hellow`
3. `cd ~/hellow`
4. `dotnet restore`
5. `dotnet run --ip 0.0.0.0`

use ip `0.0.0.0` inside container, and check docker container ip with `docker ps`
