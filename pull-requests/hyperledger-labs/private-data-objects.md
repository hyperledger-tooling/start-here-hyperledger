---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/380" class=".btn">#380</a>
            </td>
            <td>
                <b>
                    Sawtooth in-depth removal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR completes the removal of Sawtooth and depends on #379 for testing (at least the eservice) in HW mode.

This PR removes the following Sawtooth-related things:
- references in docs and toml files
- build flags and procedures
- scripts for SKF files
- configuration flags and procedures in services

Also, it updates:
- the default ledger port 8008 -> 6600
- the default ledger type sawtooth -> ccf
- the registration with the ledger -- which is now empty since CCF is not set up for checking proof-data in HW mode
- the default service keys *.skf -> *.pem
- the TransactionKeys class by deprecating the methods
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 18:56:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/379" class=".btn">#379</a>
            </td>
            <td>
                <b>
                    fix build to make CCF PDO work with the eservice (only) in SGX HW mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As we remove Sawtooth, we have a problem: CCF does not support PDO in HW mode.
This means that there is no alternative available to run PDO in SGX HW mode.

This PR partially addresses this problem:
1. it provide the docker compose material to run the CI in HW mode
2. it fixes a bug in the CCF submitters
3. in HW mode, it compiles the eservice as expected, but it forces: the pservice in sim mode, and the proof_data field to be empty. This is necessary to run (at least) the eservice in HW mode and avoid signature/field verification issues, probably due to unintended formatting. The changes (about 20 lines in 3 files) can be easily reverted as the other issues are solved.

More details of these issues are in #262 , here https://github.com/hyperledger-labs/private-data-objects/issues/262#issuecomment-1278684081.





Signed-off-by: Bruno Vavala <bruno.vavala@intel.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 08:42:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/378" class=".btn">#378</a>
            </td>
            <td>
                <b>
                    Remove Sawtooth-related files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR remove Sawtooth-related files -- many references inside other files persist.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-13 07:47:53 +0000 UTC
    </div>
</div>

