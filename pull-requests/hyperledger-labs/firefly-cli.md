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
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Update docker image paths to hyperledger repos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To make sure you always have the latest images you can run these commands:

```
docker pull ghcr.io/hyperledger-labs/firefly:latest
docker pull ghcr.io/hyperledger-labs/firefly-ethconnect:latest
docker pull ghcr.io/hyperledger-labs/firefly-dataexchange-https:latest
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 23:36:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Rename package and ethconnect headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 19:51:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Data exchange integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for https://github.com/hyperledger-labs/firefly-dataexchange-https.

Other notable improvements include:

- More error propagation throughout
- The `reset` and `remove` commands automatically perform `stop` first so you don't have to. This prevents stacks from getting into weird states where their data has been deleted but the containers themselves haven't been.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 18:11:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Add "org" to generated stack config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 21:38:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Postgres improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Move data inside containers (don't mount volumes in the data directory anymore)
- Update `reset` command to wipe containers (keeping config only)
- Fix bugs with `reset` command
- Add `-f` flag to `reset` command to force the operation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 18:02:48 +0000 UTC
    </div>
</div>

