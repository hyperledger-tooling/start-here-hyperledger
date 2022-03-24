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
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Unique topics for multiple connectors against same ethconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Few changes here:

1. We already set the topic to be unique per node in the CLI, but we don't do the same for token connectors.
    - This means if you request use of multiple token connectors of the same type, or are using the CLI to aid deployment against a remote EthConnect (such as in Kaleido), you can't be sure to have unique topics.
2. Log the API call that failed, when logging errors
3. Allow a `--contract-address` to be specified at `init`, which bypasses the contract deploy step at `start`. This can be combined with `--core-config` to use a remotely hosted EthConnect with a separately deployed contract (for example Kaleido smart contract management)
4. Remove registration of a REST API for the FireFly smart contract across all EthConnect instances, in all cases. This is no longer required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 18:35:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    Include build version using built-in Go semantics for go install
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #157 

After - doing a `go install` (so default Go build):

```sh
$ go install github.com/hyperledger/firefly-cli/ff@go-version
go: downloading github.com/hyperledger/firefly-cli v0.0.47-0.20220323122046-9483791f8c0d
$ ff version
{
  "Version": "v0.0.47-0.20220323122046-9483791f8c0d",
  "License": "Apache-2.0"
}
```

After - doing a `make` (date and commit would also be added by go-releaser):

```sh
$ make
cd ff && go build -ldflags="-X 'github.com/hyperledger/firefly-cli/cmd.BuildDate=2022-03-23T12:24:33Z' -X 'github.com/hyperledger/firefly-cli/cmd.BuildCommit=9483791'"
$ ./ff/ff version
{
  "Version": "(devel)",
  "Commit": "698c9ad",
  "Date": "2022-03-23T12:26:16Z",
  "License": "Apache-2.0"
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 12:26:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/163" class=".btn">#163</a>
            </td>
            <td>
                <b>
                    Add options for tuning ethconnect and block period
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/562
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 15:43:20 +0000 UTC
    </div>
</div>

