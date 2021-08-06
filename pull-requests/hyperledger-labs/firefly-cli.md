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

