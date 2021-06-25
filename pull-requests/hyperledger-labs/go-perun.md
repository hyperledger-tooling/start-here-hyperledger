---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Add functions to register new assets in ethereum funder implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - As these methods provide convenience for the user (to register assets after funder is initialized) and are not required by the framework itself for the process of funding, they are not added to the `Funder` interface.

- Use the `RegisterAsset` method in place of `WithDepositor`, as the newly added method provides the same functionality without making a copy of the funder.

- Also, fixed a bug in `funder_test.go`. See the last before commit for details. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 15:44:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Core82 open and close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split some more commits from #83 .

In particular, this PR includes the following:

- Open virtual channels
- Close virtual channels
- Test virtual channels happy case
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 14:16:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    Fix testHashState
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test the HashState function instead of CalcID, which is already being tested in testCalcID.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 11:22:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    Prep82 update bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split some more commits from #83 .

In particular, this PR includes the following:
- Update contract bindings
- Adopt channel data types
- registerRecursive
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 15:46:47 +0000 UTC
    </div>
</div>

