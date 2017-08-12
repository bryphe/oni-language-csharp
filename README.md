# oni-language-csharp
## C# Language Plugin for [Oni](https://github.com/extr0py/oni) 

C# completion for Oni uses the [OmniSharp Node Client](https://github.com/OmniSharp/omnisharp-node-client) which provides language capabilities for both .NET and Mono. For it to work correctly, you need to have a valid `.csproj` file with any dependent packages (ie, Nuget) installed. The project should also build and compile.

## Usage

To get started:

- Clone repository into your oni plugin path (~/.oni/plugins)
- Run `npm install`

## Features

- Goto Definition
- Error Highlights
- Code Completion

## Known Issues

- On Windows, you must run Oni as an administrator the first time using the C# language service. This is tracked by issue [#423](https://github.com/extr0py/oni/issues/423).
- On all platforms, the C# language service takes time to start up, especially the first time as it is downloading the appropriate runtime environment. You can open up the developer tools (Help -> Developer Tools) to see the logging from the language service.
