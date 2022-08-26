---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/989" class=".btn">#989</a>
            </td>
            <td>
                <b>
                    WIP: Feature ink metadata for substrate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                attempt to generate ink compatible metadata using ink_metadata::InkProject
currently relies on unmerged branched of scale-info, ink_metadata.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 07:35:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/988" class=".btn">#988</a>
            </td>
            <td>
                <b>
                    Multiplication overflow detection for integer width > 64 bits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: salaheldinsoliman <salaheldin_sameh@aucegypt.edu>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 03:15:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/987" class=".btn">#987</a>
            </td>
            <td>
                <b>
                    Create 'writeStringData' and 'writeBytesData'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates `writeStringData` and `writeBytesData` functions that write only the contents of strings and bytes arrays into a buffer. They are useful for using bincode when creating a library for System Instructions on Solana.

For arrays (strings and bytes included) bincode encodes lengths in `u64`, so borsh encoding cannot be used for this case.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 19:31:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/985" class=".btn">#985</a>
            </td>
            <td>
                <b>
                    Generate solidity interface from Anchor IDL files so that anchor contracts can be called
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
        Created At 2022-08-23 18:59:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/983" class=".btn">#983</a>
            </td>
            <td>
                <b>
                    Always run linux arm64 tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Thanks for Hyperledger, we now have an mac m1 running asahi linux which we can use for linux arm64 tests and builds.

Now also run the tests on pull requests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 11:17:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/982" class=".btn">#982</a>
            </td>
            <td>
                <b>
                    Multiplication overflow detection for types of size more than 64 bits.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Multiplication overflow detection for bits > 64.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 08:13:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/981" class=".btn">#981</a>
            </td>
            <td>
                <b>
                    Remove ewasm target and rename usable parts for evm target
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Ethereum Foundation has stopped funding for ewasm work, so it is
unlikely to happen in the current form. In addition, burrow has been end
of life'd by Hyperledger. So, the ewasm target is no longer useful.

We would love to have an evm target at some point in the future. Many
parts of the ewasm target is re-usable for evm, so we rename ewasm to
evm and remove the parts which are irrelevant for evm.

Note that the new evm target is good enough for the language server, so
the language server can be started in evm mode:

```
solang language-server --target evm
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 16:42:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/980" class=".btn">#980</a>
            </td>
            <td>
                <b>
                    Make lexer public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exposing the lexer API would be useful for things like syntax highlighting. Plus its implemented clean as is to be exposed directly :hugs: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 16:05:55 +0000 UTC
    </div>
</div>

