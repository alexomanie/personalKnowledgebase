# App Service Deploy

There are several ways to deploy an App Service

## Deploy directly from a ZIP file

when you run directly from a package, the files in the package are not copied to the wwwroot directory. Instead, the ZIP package itself gets mounted directly as the read-only wwwroot directory

### Possible benefits

- Eliminates file lock conflicts between deployment and runtime.
- Ensures only full-deployed apps are running at any time.
- Can be deployed to a production app (with restart).
- Improves the performance of Azure Resource Manager deployments.
- May reduce cold-start times, particularly for JavaScript functions with large npm package trees.
