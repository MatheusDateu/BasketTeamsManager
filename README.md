# Technologies
The project was developed using the following technologies:

- Blazor WebAssembly - A web framework for creating interactive user interfaces using C# and WebAssembly.
- Bootstrap - A CSS framework for creating responsive and custom layouts.

## Installation
To run the project locally, you need to have the following installed on your machine:

- .NET 6.0 SDK - The .NET software development kit, which includes the runtime, tools, and necessary libraries.
- Python 3 - An interpreted, high-level, general-purpose programming language that will be used to start a static web server.

After installing the requirements, you can clone the project repository using the command:

```bash
git clone https://github.com/mdelmondes/BasketMatchManager.git
```

Then, you can publish the project using Visual Studio or the command:

```bash
dotnet publish -c Release
```

This will generate a `publish` folder with the project's static files in the `wwwroot` folder.

## Execution
To run the project, you need to start a static web server in the `wwwroot` folder. You can do this using the command:

```bash
python -m http.server --directory {path}\wwwroot
```

Where `{path}` is the path to the folder containing the static files. For example, if the folder is in `C:\Projects\WASM`, you can use:

```bash
python -m http.server --directory C:\Projects\WASM
```

This will start a server on the default port 8000, and you can access the project in the browser using the address http://localhost:8000. You can change the port using an additional argument, for example:

```bash
python -m http.server 5000 --directory C:\Projects\WASM
```

This will start the server on port 5000, and you can access the project at the address http://localhost:5000.

## Tests
To run the project tests, you can use Visual Studio or the command:

```bash
dotnet test
```

This will run the unit and integration tests of the project using the xUnit framework.

To check the code quality, you can use the command:

```bash
dotnet format
```

This will format the code according to the conventions of the EditorConfig.

## Contribution
If you want to contribute to the project, whether by fixing bugs, adding new features, or providing suggestions, you can:

- Open an issue on GitHub, explaining the problem or proposal.
- Fork the repository, make the necessary changes, and submit a pull request to the main branch.

## Authors
The project was developed by:

- **Matheus Delmondes** - Developer and project ideator.

## License
The project is under the MIT license, which allows the use, copying, modification, and distribution of the code, provided that copyrights and permissions are maintained.
