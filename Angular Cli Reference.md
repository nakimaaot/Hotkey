# Angular CLI Reference
---
ng new
---
`ng new <project-name> [options]`

Creates a new Angular project. By default, the project is created under
the current directory.  

Option | Description
--- | ---
--dry-run | only output the files created and operations performed, do not actually create the project. Alias: 'd'.
--verbose | output more information. Alias: 'v'.
--skip-npm | do not run any npm command once the project is created.
--skip-git | do not create a git repository for the project.
--directory | parent directory to create the new project into.

ng init
---
`ng init <project-name> [options]`

Creates a new Angular project in the current folder.

Option | Description
--- | ---
--dry-run | only output the files created and operations performed, do not actually create the project. Alias: 'd'.
--verbose | output more information. Alias: 'v'.
--skip-npm | do not run any npm command once the project is created.
--name | The name of the project to create.

ng completion
---
`ng completion`
Adds autocomplete functionality to your shell for ng commands.

ng e2e
---
`ng e2e`
Runs all end-to-end tests defined in your application, using protractor.

ng format
---
`ng format`
Formats the code of this project using clang-format.

ng doc
---
`ng doc <keyword>`
Opens a browser window with the keyword as search in Angular documentation.

ng generate
---
`ng generate <type> [options]`

Generate new code inside your project.  
Alias: 'g'

Valid types:

Option | Description
--- | ---
`component <path/to/component-name>` | Generates a component.
`directive <path/to/directive-name>` | Generates a directive.
`route <route/to/route-component>` | Generates a route. The name should be the route used in the RouteConfig.
`pipe <path/to/pipe-name>` | Generates a pipe.
`service <path/to/service-name>` | Generates a service.

The generated component has its own directory, unless the --flat options
is specified.

Option | Description
--- | ---
--flat | Do not create the code in its own directory.
`--route=<route>` | Specify the parent route. Only for generating components and routes. Default to the path specified.
--skip-router-generation | Skip generating the route config for the parent. Only usable for routes.
--default | Specify that the route should be a default route.
--lazy | Specify that the route is lazy. Default to true.

ng get
---
`ng get <path1, path2, ...pathN> [options]`

Get a value from the Angular CLI configuration. The pathN arguments is a valid
JavaScript path like "users[1].userName". If the value isn't set, "undefined"
will be shown. This command by default only works inside a project directory.

Options:

Option | Description
--- | ---
--global | Returns the global configuration value instead of the local one (if both are set). This option also makes the command work outside of a project directory.

ng set
---
`ng get <path1=value1, path2=value2, ...pathN=valueN> [options]`

Set a value in the Angular CLI configuration. By default, sets the value
in the project's configuration if ran inside a project, or fails if not
inside a project. The pathN arguments is a valid JavaScript path like
"users[1].userName". The value will be coerced to the proper type or will
throw an error if the type cannot be coerced.

Options:

Option | Description
--- | ---
--global | Sets the global configuration value instead of a local one. This also makes `ng set` works outside a project.

ng github-pages:deploy
---
`ng github-pages:deploy [options]`

Build the application for production, setup the GitHub repository, then publish the app.

Options:

Option | Description
--- | ---
`--message=<message>` | Commit message to include with the build. Defaults to "new gh-pages version".
`--environment=<env>` | The Angular environment to build. Defaults to "production".
`--branch=<branch-name>` | The git branch to push the pages to. Defaults to "gh-branch".
`--skip-build` | Skip building the project before publishing.
`--gh-token=<token>` | API token to use to deploy. Required.
`--gh-username=<username>` | The Github username to use. Required.

ng lint
---
`ng lint`
Run the codelyzer linter on your project.

ng test
---
`ng test [options]`
Run unittests, using karma.

Options:

Option | Description
--- | ---
--watch | Keep running the tests. Default to true.
--browsers, --colors, --reporters, --port, --log-level | Those arguments are passed directly to karma.

ng version
---
`ng version`

Outputs the version of angular-cli, node and the operating system.


