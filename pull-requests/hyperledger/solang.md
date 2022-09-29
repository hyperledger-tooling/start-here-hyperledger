---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1025" class=".btn">#1025</a>
            </td>
            <td>
                <b>
                    Update seal calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">substrate</span>
            </td>
            <td>
                This PR updates the `seal_` calls to reflect newer versions. Some of them use `seal1` and some storage APIs  temporarily  `__unstable__`now (will be changed as soon as they are released to some stable version).
Individual calls updated:
- `seal_random`: Returns 4 more bytes (the block number) so the output buffer size had to be extend
- `seal_instantiate`: Args changed
- `seal_terminate`: Args changed
- `seal_call`: Args (flags can be done later if needed)
- `seal_set_storage`: Signature changed. `key_len` will be needed for transparent hashing, once we fix the metadata generation. The newly introduced return type (the length of the pre-existing value, if any) is ignore for now since in solidity we don't use that.
- `seal_clear_storage`: Same as above.
- `seal_get_storage`: Arguments changed

Additionally I decided to introduce a few macros to get rid of some awkward and repeating patterns and make it easier to reason about the emitted code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 20:06:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1024" class=".btn">#1024</a>
            </td>
            <td>
                <b>
                    constant overflow compatible with solc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR evaluates expressions constant arithmetic and checks for overflow according to what Solc does

Signed-off-by: salaheldinsoliman <salaheldin_sameh@aucegypt.edu>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-26 11:50:47 +0000 UTC
    </div>
</div>

