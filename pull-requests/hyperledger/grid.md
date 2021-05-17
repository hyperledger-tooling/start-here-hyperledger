---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/696" class=".btn">#696</a>
            </td>
            <td>
                <b>
                    Run cron builds at 1am
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cron builds running at 2am are failing regularly. Moving the build to
run earlier will either fix the problem or disprove a theory.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 16:23:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    List and show agents in the CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes man-pages. List includes formatting human and csv types, along
with the ability to list roles on their own lines. The Show command
gives additional information, and requires a public key as the
identifier. (Agent ID is synonymous with public key.)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 17:42:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/690" class=".btn">#690</a>
            </td>
            <td>
                <b>
                    Add GDSN support for CLI update, tests, and documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR cleans up some loose ends from the GDSN support feature:

- Implement product update in the CLI for multiple files and GDSN files
- Removing some unused code
- Adding unit tests to the GDSN module
- Adding docstrings to the GDSN module
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 16:46:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Cache dependencies for all features in grid-dev
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 18:25:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/686" class=".btn">#686</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-1:  Fix Grid docker builds with Docker Compose 1.28+
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As of version 1.28.0, Docker Compose expects .env files to reside in the same
directory as the compose files or to have their path specicified with an
additional argument to the compose command. Duplicating the .env files
whereever they're needed was deemed to be the least disruptive solution.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 22:20:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    Fix Grid docker builds with Docker Compose 1.28+
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
        Created At 2021-05-10 18:52:45 +0000 UTC
    </div>
</div>

