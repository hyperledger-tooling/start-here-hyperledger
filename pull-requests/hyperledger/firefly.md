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
                PR <a href="https://github.com/hyperledger/firefly/pull/1137" class=".btn">#1137</a>
            </td>
            <td>
                <b>
                    Add FIR-16 enhancements to fftokens documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document the new parameters and APIs that were added as part of [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 17:06:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1136" class=".btn">#1136</a>
            </td>
            <td>
                <b>
                    Fix: typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: typos

Signed-off-by: omahs <73983677+omahs@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 15:52:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    Check variable before using its value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a check to see if poolData is nil before attempting to access its fields. 

Resolves #1121 

Signed-off-by: Ayushya Chitransh <ayushyachitransh@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 12:24:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    Fix coverage gap in FFIErrors, and make DB interface consistent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There was no coverage of the DB interface for FFI Errors, and oddly there was a difference in the query interface to all other DB packages. Unsure why that was, so I made it consistent.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 19:15:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    Add DELETE method for data API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on: https://github.com/hyperledger/firefly-dataexchange-https/pull/73
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 21:24:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    Add docs on passing ABI info to token pools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16).

This links out to the READMEs of both token connectors for "more details", so these PRs are relevant to be merged alongside this one:
https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/108
https://github.com/hyperledger/firefly-tokens-erc1155/pull/107
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 20:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1130" class=".btn">#1130</a>
            </td>
            <td>
                <b>
                    Add strong nil checking on orchestrator and redress test coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixes #1116
   - I went the route of forcing `nil` checking on the `Operator()` method everywhere (apart from unit tests, where I added a `MustOrchestrator`)
- Addresses a couple of  areas where test coverage seems to have slipped

After fix:
![image](https://user-images.githubusercontent.com/6660217/210892935-f458ab7a-6b8e-46a4-9398-5cd2217c2764.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 22:34:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1129" class=".btn">#1129</a>
            </td>
            <td>
                <b>
                    Add docs on fftokens
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <img width="1234" alt="fftokens_-_Hyperledger_FireFly_Docs" src="https://user-images.githubusercontent.com/1993829/210884637-4b4a3027-4e8c-4e6c-a5b4-ecc2e5d4f288.png">

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 21:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1126" class=".btn">#1126</a>
            </td>
            <td>
                <b>
                    remove XDC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 16:47:30 +0000 UTC
    </div>
</div>

