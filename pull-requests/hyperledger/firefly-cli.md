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
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Using Renamed FFDX Plugin for Dataexchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: hfuss <haydenfuss@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 00:53:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Add memory warning with stacks of more than 3 members
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly-cli/issues/150

Unfortunately there does not appear any way to easily programmatically set the Docker VM to use more memory, and the default (2 GB) is pretty lows for running the number of processes required to run a FireFly stack.

When a stack with more than 2 members (1 GB per member) is initialized, this prints a warning noting that the default may need to be increased.

As a future enhancement, it would be nice if this warning was only printed if not enough RAM was allocated, but that would require knowing how much RAM the Docker VM currently has allocated. I couldn't find a quick way to do that yet.

Note: This is not an issue on Linux, because Docker doesn't run in a VM on Linux.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 20:32:52 +0000 UTC
    </div>
</div>

