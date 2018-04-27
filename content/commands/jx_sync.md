---
date: 2018-04-27T04:28:28Z
title: "jx sync"
slug: jx_sync
url: /commands/jx_sync/
---
## jx sync

Synchronises your local files to a devpod

### Synopsis

Synchronises your local files to a devpod so you an build and test your code easily on the cloud

```
jx sync [flags]
```

### Examples

```
  # Open a terminal in the first container of the foo deployment's latest pod
  jx sync foo
```

### Options

```
  -c, --container string    The name of the container to log
  -d, --dir string          The directory to watch. Defaults to the current directory
  -h, --help                help for sync
  -n, --namespace string    the namespace to look for the Deployment. Defaults to the current namespace
  -p, --pod string          the pod name to use
      --reload              Should we reload the remote container on file changes?
  -r, --remote-dir string   The remote directory in the DevPod to sync (default "/code")
  -s, --shell string        Path to the shell command (default "/bin/sh")
```

### SEE ALSO

* [jx](/commands/jx/)	 - jx is a command line tool for working with Jenkins X

###### Auto generated by spf13/cobra on 27-Apr-2018