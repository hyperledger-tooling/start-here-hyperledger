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
                PR <a href="https://github.com/hyperledger/solang/pull/1027" class=".btn">#1027</a>
            </td>
            <td>
                <b>
                    Function name mangling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implement function name mangling in sema.

I used the simplest mangling algorithm possible: I think that basically re-using the `.signature` field of the function fits our use case well here:
* It should already be unique for each function
* Return values do not matter in the distinction of overloaded functions (in solidity the arguments must still be different).
* The mangled function names are very user friendly, since they contain the name together with the argument types.

But I might be missing something here, I'm open to change this if there is a better solution.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 12:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1026" class=".btn">#1026</a>
            </td>
            <td>
                <b>
                    Use partition_point() rather than a hand-rolled linear scan
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                First, this fixes a problem in the file offset to line/column number conversion. This happens if the offset lands exactly on the newline.

Secondly, this replaces a linear scan with [partition_point](https://doc.rust-lang.org/std/primitive.slice.html#method.partition_point).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 12:13:45 +0000 UTC
    </div>
</div>

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

