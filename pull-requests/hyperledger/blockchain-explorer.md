---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/302" class=".btn">#302</a>
            </td>
            <td>
                <b>
                    Drop EXPOSE from Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow-up for #301; not useful if that is rejected.

There doesn't seem to be a good way to make this respect a param or
envvar passed in, and it's not strictly *needed* if you're mapping ports.

Having it be present & incorrect in some cases is worse than having it
be absent in some cases where it would be correct. So just drop it
entirely.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 18:52:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/301" class=".btn">#301</a>
            </td>
            <td>
                <b>
                    Make port 8080 parameterized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This drastically simplifies using this image with different networks, which frequently will include a container which uses port 8080.

Changing this container to support other port numbers is frequently going to be simpler than modifying the network the explorer is attaching to, and centralizing it in one place is *definitely* simpler than having every Explorer user make the changes themselves.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 18:44:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    Two small tweaks for ease of use
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - script that exports DB settings from `app/explorerconfig.json` to the envvars, which makes it easier to use the example commands in the Quick Start
- script and doc tweaks to make it clear that `npm start` runs the app only while the process continues rather than in detached mode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 23:15:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Customize Quick-Start docs by OS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Commands and portions of results are different on Linux vs. MacOS, and this is not reflected in the docs. Updated to correct that.

Also, add a small piece explaining how to generate a new Docker image from this repository. It already doesn't use the same name as the canonical image (`hyperledger-explorer` rather than `hyperledger/explorer`), so this is not going to pollute the image repository and is unlikely to cause confusion unless someone deliberately tries to mess with it.

The second part is useful for developers who want to test changes to the image and/or create forks of the project. It would have saved me some time - I made an unwarranted assumption about the local install/build process also creating images and took a while to correct that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 23:03:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    daysToKeep deprecation - keep daily logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The log option 'daysToKeep' is deprecated without any replacement available. Suggested change is to use `numBackups`; unfortunately, `maxLogSize` generates an unpredictable number of logs per time, so ensuring that a full week of logs is retained is incompatible with the migration. (A possible workaround would be setting `numBackups: 1000000000`, or some other ludicrously-high value, but even this isn't perfectly guaranteed to include a full week if something goes wrong that generates a massive amount of logs.)

This change will eventually be necessary. Currently it is not, but leaving the deprecation present generates a long list of warnings when built (true since #272); this will suppress those.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 21:35:37 +0000 UTC
    </div>
</div>

