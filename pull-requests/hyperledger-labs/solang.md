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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/968" class=".btn">#968</a>
            </td>
            <td>
                <b>
                    Introduce new syntax for overriding selector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This introduces syntax like so:
```
function get_foo() selector=hex"01020304" public return (int) {
    return 102;
}
```
Note this functionality will be used in a following commit to define interfaces derived from anchor idl files. Tests or Solana will be in that PR, no changes as the functionality will change in that PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 10:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/963" class=".btn">#963</a>
            </td>
            <td>
                <b>
                    add shell completions for cli app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `shell-complete` sub-command, allowing users to autocomplete our CLI with the TAB key (this pretty much defuses the issue of typing full length sub-commands out all the time). As a bonus It also shows remaining options when there is nothing to complete yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-14 13:20:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/961" class=".btn">#961</a>
            </td>
            <td>
                <b>
                    WIP: Create abi.borshDecode method for Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates the Borsh decoding for Solana. It is still a work in progress.

- [x] Write the decoding algorithm
- [x] Create codegen tests
- [x] Create runtime tests
- [x] Create tests with invalid data
- [x] Remove duplicate code
- [ ] Clean up the mess I made myself
- [ ] Write doc comments


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 20:38:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/959" class=".btn">#959</a>
            </td>
            <td>
                <b>
                    Make --generate-debug-info hidden
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature is incomplete and does not have any users yet. For example, there is a debugging endpoint for Solana in the works, but this is not finished yet. Also, this will be useful for static analysis, which requires debug information for higher-level type information.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 08:39:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/958" class=".btn">#958</a>
            </td>
            <td>
                <b>
                    Update roadmap for Substrate target
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @athei we are reworking the solang roadmap. I mapped  the milestones from the solang Bounty Proposal into the roadmap as follows:
- V0.2: Includes Milestones 1, 2, 3, 4, 6
- V0.3: Includes Milestones 5, 7, 8, 9
- V0.4: Includes Milestones 10, 11

Of course nothing will be set in stone here. What do you think?

Signed-off-by: Cyrill Leutwiler <bigcyrill@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 20:40:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/957" class=".btn">#957</a>
            </td>
            <td>
                <b>
                    Bytes of Type::Bytes must be reversed before encoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Type::Bytes` is represented as an integer in LLVM. This means its bytes are reversed if we use the `Instr::WriteBuffer` instruction. This PR fixes this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 18:49:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/956" class=".btn">#956</a>
            </td>
            <td>
                <b>
                    Introduce cli subcommands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fits the CLI more natural.

Now we have:

solang compile --target .. file..
solang language-server --target ..
solang doc --target .. file..

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 13:43:45 +0000 UTC
    </div>
</div>

