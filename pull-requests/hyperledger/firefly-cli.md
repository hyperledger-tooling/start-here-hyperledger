---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Set default connector to evmconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/1135
Resolves https://github.com/hyperledger/firefly-cli/issues/233
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 21:21:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    first draft for supporting docker-compose v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Pull Request

## Disclaimer

I'm not a golang developer, so any code presented here is a collection of educated guesses as how to solve the problem.
With that out of the way, let's present the pull request.

## Problem
This pull request adresses [Issue231: firefly fails check for docker compose v2](https://github.com/hyperledger/firefly-cli/issues/231). The problem arises due to docker changing the syntax for docker-compose from `docker-compose` in version 1 to `docker compose` in version 2. There is always the workaround to require the standalone docker-compose in version 1.

## Fix

The fix is split into two parts, adressing the checking of the version and integrating the information into the stack manager that executes the docker commands via `RunDockerComposeCommand`. The information about which version syntax to use for the commands is carried via context.

### CheckDockerConfig
the function that checks for the prerequisites when executing docker-compose commands, `CheckDockerConfig` returns a tuple `(DockerComposeVersion, error)` with `DockerComposeVersion` as enum to differentiate between `None`, `ComposeV1` and `ComposeV2`. This value is stored in a context that is later transferred into the stack manager.
Unfortunately, cobra with version 1.4.0 does not provide the capability to allow context to be attached to a command.
Only from version 1.5.0, this feature has been merged, for reference: [support for SetContext](https://github.com/spf13/cobra/pull/1551).
The solution using cobra 1.5.0 concerns all commands which use both `PreRunE` and `RunE` while also requiring the docker compose version to be transferred as context between these two executions:

```go 
        PreRunE: func(cmd *cobra.Command, args []string) error {
		ctx := ...
		version, err := docker.CheckDockerConfig()
		ctx = context.WithValue(ctx, docker.ComposeVersion{}, version)
		cmd.SetContext(ctx)
		return err
	},
	RunE: func(cmd *cobra.Command, args []string) error {
                ...
		stackManager := stacks.NewStackManager(cmd.Context())
               ...
	},
```

The functions currently affected are defined in:
- `accounts_create.go`
- `accounts_list.go`
- `deploy_ethereum.go`
- `deploy_fabric`

No version update is required when simply combining both executions, similar to functions from:
- `info.go`
- `logs.go`
- `reset.go`
- `start.go`

```go 
        RunE: func(cmd *cobra.Command, args []string) error {
		ctx := ...
		version, err := docker.CheckDockerConfig()
		ctx = context.WithValue(ctx, docker.ComposeVersion{}, version)
                if err != nil {
                     return err
                }
		stackManager := stacks.NewStackManager(cmd.Context())
               ...
	},
```

### RunDockerComposeCommand

The second part of the changes affects the way the stack manager runs docker-compose functions. By retrieving the docker-compose version, either `docker-compose` or `docker compose` can be executed

## Possible Tweaks

- Instead of storing a version in the context, the command itself can be stored; when docker-compose in version 2 is detected, instead storing V1, the string `docker compose` is attached to the context with `ComposeCmd` as key. Consequently, the `RunDockerComposeCommand` function simply executes `exec.Command(ctx.Value(ComposeCmd{}), command...)`.

## Open Question

- Is the separation between `PreRunE` and `RunE` necessary, because currently only docker checks are executed in `PreRun`. Small commands do not even specify `PreRunE` at all.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 01:22:56 +0000 UTC
    </div>
</div>

