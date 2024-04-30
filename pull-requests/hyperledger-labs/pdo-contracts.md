---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    Consistent (& bug-fixed) sub-module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Should solve the issue Prakash run into this morning regarding docker target `build_pdo_images` and also fixes a bug from PR #38.  While testing i run again in [my issues from PR #32](https://github.com/hyperledger-labs/pdo-contracts/pull/32#pullrequestreview-2007629098), although the first item could be traced now to having a space in a token class which is not handled/supported and the second is some so-far-unavoidable,-known-and-ignorable issue.  Didn't revisit the third bullet regarding earlier unresolved things as i guess we will revisit them (if still existing) once we start more systematic scenario testing (see issue #39) ...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 23:27:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    Add dependabot to track submodule deps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR allows dependabot to take the burden and bump the gitsubmodule version of PDO automatically. 

An example can be found in my fork https://github.com/mbrandenburger/pdo-contracts/pulls

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 19:01:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/38" class=".btn">#38</a>
            </td>
            <td>
                <b>
                    Parameterize docker(-compose) commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Companion to [PDO PR #487](https://github.com/hyperledger-labs/private-data-objects/pull/487)  . See there for more context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 21:33:43 +0000 UTC
    </div>
</div>

