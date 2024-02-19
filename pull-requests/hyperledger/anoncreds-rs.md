---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    mark Python wrapper as not under construction anymore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Berend Sliedrecht <sliedrecht@berend.io>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 11:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/329" class=".btn">#329</a>
            </td>
            <td>
                <b>
                    chore: update version for js wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updating version to 0.2.1 after #327. Only for the JS wrapper, as I understand we follow the same strategy as in Askar and Indy VDR. I think @TimoGlastra in #296 did already the set-up so it will be just a matter of running the workflow manually.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 22:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    Deal with snyk notifications for react-native -- by updating to latest of all dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In making this PR, I looked up the latest versions of each of the called out in the Snyk report and used that.  We'll see how that goes.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 20:34:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    fix(rn): update libanoncreds headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I was updating my react-native app to last credo alpha (which uses anoncreds-rs 0.2.0) and wasn't able to build in any OS due to a type error. It seems that the libanoncreds.h header wasn't updated after the changes in https://github.com/hyperledger/anoncreds-rs/pull/320.

I've regenerated the file using `cbindgen` and noticed several changes (like comments and some methods that were missing), so I guess it has been modified manually lately.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 22:03:29 +0000 UTC
    </div>
</div>

