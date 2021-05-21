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
                PR <a href="https://github.com/hyperledger/grid/pull/704" class=".btn">#704</a>
            </td>
            <td>
                <b>
                    Fix typos in Pike smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change fixes several typos present in the Pike smart contract's
`handler` module.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 20:14:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/702" class=".btn">#702</a>
            </td>
            <td>
                <b>
                    Fix  typos and formatting issues in Grid Pike smart contract
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
        Created At 2021-05-20 19:28:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    Have only one DEFAULT_GRID_PROTCOL_VERSOIN const
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Banks <rbanks@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 18:47:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/698" class=".btn">#698</a>
            </td>
            <td>
                <b>
                    Update signer to match splinter's pattern
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
        Created At 2021-05-19 19:05:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/697" class=".btn">#697</a>
            </td>
            <td>
                <b>
                    Refactor pike protocol payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PikePayload protocol object now has a single action object instead of
multiple payload objects. The Action enum has been updated to hold a
payload object that corresponds to each enum type.

Signed-off-by: Ryan Banks <rbanks@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 16:27:37 +0000 UTC
    </div>
</div>

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

