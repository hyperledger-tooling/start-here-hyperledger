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
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    adding binary builds via goreleaser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This new action will be triggered on PR's, pushes to master, and new tags.

I'm including PR's and pushes to master so we can verify builds. GoReleaser will **only** publish releases if the commit it's building is associated with a tag.

closes https://github.com/hyperledger-labs/firefly-cli/issues/58
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 01:55:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/72" class=".btn">#72</a>
            </td>
            <td>
                <b>
                    Ensure ethereum accounts unlocked before proceeding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix timing issues running the CLI in GitHub actions or other slower environments
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-02 21:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Automatically rollback failed first time setup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Add --no-rollback -b flag to change new rollback default behavior
* Add 60 second timeout on member registration
* Clean up logging on stack startup

Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>

closes #70 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-02 15:06:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Create stack and config optimized for running a FireFly core outside of docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes it easy(er) to run one or more FireFly core processes outside of docker. This is especially useful when making code changes to FireFly itself and wanting to step through the code in a debugger.

You can now use the `-e <int>` flag to specify the number of core processes that you would like to manage outside of docker. The default (if `-e` is not set) is `0`, meaning that unless `-e` is set, all FireFly core processes will run inside docker.

When starting a stack with external processes, the CLI will wait for FireFly to run before running contract deployment and member registration. This means that the developer doesn't have to worry about complex registration even when they are debugging FireFly locally. This should greatly speed up local development going foward.

> **NOTE**: Right now it is a requirement that _at least one_ FireFly core run inside docker, because the CLI needs to pull the compiled smart contracts out of a container to install them

Resolves https://github.com/hyperledger-labs/firefly-cli/issues/39
Resolves https://github.com/hyperledger-labs/firefly-cli/issues/2

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 14:05:24 +0000 UTC
    </div>
</div>

