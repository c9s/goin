goin - Go Package Installer
===========================

package structure:

    src/  # main package source code
    vendor/src  # vendor packages

package info spec is stored in the `goin.json` file:

```json
{
    "name": "goin",
    "version": "1.0.0",
    "go": {
        "version": 1.1
    },

    // define package dependency
    "require": {
        // install as a remote package
        "github-client": { "remote": "github.com/alcacoop/go-github-client/users" },

        // install as a local package, so you can import these packages as local packages.
        "net/github": { "local": "git@github.com:alcacoop/go-github-client.git" }
    }
}
```


