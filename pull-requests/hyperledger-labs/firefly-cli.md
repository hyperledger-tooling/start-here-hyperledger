---
layout: default
title: firefly-cli
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    only show badge for main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:28:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    add build workflow badge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:17:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    Fix bugs with initialization and starting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes:

- PostgreSQL always being selected regardless of command line arguments
- SIGSEGV when using an external node
- SIGSEGV when using an external node with postgres
- Startup sequence not listening on correct port for external processes on first time startup
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 17:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Blockchain refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR shouldn't have any effect on the actual functionality of the CLI from an end user perspective, but it is required to support multiple different blockchains.

The main change here is that there is now a `StackManager` (much of the existing `stacks.go` code) which uses an `IBlockchainProvider` interface to set up the stack. The interface looks like this:

```go
type IBlockchainProvider interface {
	WriteConfig() error
	RunFirstTimeSetup() error
	DeploySmartContracts() error
	PreStart() error
	PostStart() error
	GetDockerServiceDefinitions() []*docker.ServiceDefinition
	GetFireflyConfig(m *types.Member) *core.BlockchainConfig
}
```

The blockchain provider implementation is now responsible for generating Docker compose sections for each container as well as the FireFly core config for the `blockchain` section of the config file. There are also functions that will be called at various points in the stack lifecycle:

- `RunFirstTimeSetup()`: Runs _before_ any docker services are started for the very first time. This is useful for copying config files to volumes.
- `DeploySmartContracts()`: Runs after the docker services have been started for the first time. This is where the blockchain provider implementation should deploy all of the contracts that it needs
- `PreStart()`: Runs before the docker services start every time
- `PostStart()`: Runs after the docker services start every time

Other miscellaneous changes include just shuffling code around for better organization and preventing import cycles.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 13:39:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Minor enhancements to contract/REST calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are the commits originally in #79 but not specifically related to tokens.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 15:08:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Deploy ERC1155 contract and tokens microservice
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tokens Docker will need to be deployed before this can work, which implies a dependency on https://github.com/hyperledger-labs/firefly-tokens-erc1155/pull/3. **Edit:** this pre-req is now [done](https://github.com/hyperledger-labs/firefly-tokens-erc1155/pkgs/container/firefly-tokens-erc1155).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 12:45:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Add command line flag for customizing provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a start for support for several different blockchain providers. This just adds the command line interface options to specify which provider you want. `geth` is the only valid option currently. It's also written to the `stack.json` now so future versions of the CLI should be able to read `stack.json` files created with this code and be able to load that stack.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 20:16:35 +0000 UTC
    </div>
</div>

