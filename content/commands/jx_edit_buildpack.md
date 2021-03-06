---
date: 2019-01-07T20:37:53Z
title: "jx edit buildpack"
slug: jx_edit_buildpack
url: /commands/jx_edit_buildpack/
---
## jx edit buildpack

Edits the build pack configuration for your team

### Synopsis

Edits the build pack configuration for your team

```
jx edit buildpack [flags]
```

### Examples

```
  # Edit the build pack configuration for your team, picking the build pack you wish to use from the available
  jx edit buildpack
  
  # to switch to classic workloads for your team
  jx edit buildpack -n classic-workloads
  
  # to switch to kubernetes workloads for your team
  jx edit buildpack -n kubernetes-workloads
  
  For more documentation see: [https://jenkins-x.io/architecture/build-packs/](https://jenkins-x.io/architecture/build-packs/)
```

### Options

```
  -b, --batch-mode                In batch mode the command never prompts for user input
      --headless                  Enable headless operation if using browser automation
  -h, --help                      help for buildpack
      --install-dependencies      Should any required dependencies be installed automatically
      --log-level string          Logging level. Possible values - panic, fatal, error, warning, info, debug. (default "info")
  -n, --name string               The name of the BuildPack resource to use
      --no-brew                   Disables the use of brew on macOS to install or upgrade command line dependencies
      --pull-secrets string       The pull secrets the service account created should have (useful when deploying to your own private registry): provide multiple pull secrets by providing them in a singular block of quotes e.g. --pull-secrets "foo, bar, baz"
  -r, --ref string                The Git reference (branch,tag,sha) in the Git repository to use
      --skip-auth-secrets-merge   Skips merging a local git auth yaml file with any pipeline secrets that are found
  -u, --url string                The URL for the build pack Git repository
      --verbose                   Enable verbose logging
```

### SEE ALSO

* [jx edit](/commands/jx_edit/)	 - Edit a resource

###### Auto generated by spf13/cobra on 7-Jan-2019
