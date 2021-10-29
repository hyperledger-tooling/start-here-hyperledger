---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Update GitHub actions to build every merge to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new GitHub action to build a docker image for every merge to `main`, but it is not designated as a "release" on GitHub. This allows us to use and test any commit, but won't clutter up our releases page. The image will be tagged with a date-stamped release number, and the newest build will also be tagged with `head`. This means if someone wants the latest, bleeding edge build of firefly, the can just pull `docker pull ghcr.io/hyperledger/firefly:head` and they will get whatever is the latest commit in `main.

The images area also labeled (separate from being tagged) with the Git commit that they were built from, as well as the date and build number.

The `manifestgen.sh` script also gets an update with this, allowing it to pull the `head` tag for all services and create a `manifest.json` with those images. To do this, run:

```
./manifestgen.sh head
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 19:47:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Update DX dependency, and go deps including bluemonday for CVE-2021-42576
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updates dependencies for security issues
- Pulls in all the latest images of downstream deps
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 15:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Update docs and add new guides
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Contributor's Guide has seen some meaningful updates in this PR. There are some additional, brand new guides added here too.

Relevant changes can be previewed here:

- Contributor's Guide: https://nguyer.github.io/firefly/contributors/contributors.html
- Contributing to Documentation: https://nguyer.github.io/firefly/contributors/docs_setup.html
- Advanced CLI Usage: https://nguyer.github.io/firefly/contributors/advanced_cli_usage.html
- Versioning Scheme: https://nguyer.github.io/firefly/maintainers/version_scheme.html
- Release Guide: https://nguyer.github.io/firefly/maintainers/release_guide.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 20:23:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Replace BeforeSend callback with a Prepare method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This instructs the sender to prepare the message for sending, but return before
actually sending it. Re-invoking Send or SendAndWait on the same sender should
dispatch the prepared message.

Further aligned methods between transfers and messaging for consistency.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 16:05:29 +0000 UTC
    </div>
</div>

