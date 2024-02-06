---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6510" class=".btn">#6510</a>
            </td>
            <td>
                <b>
                    Gha test report permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                testing permissions on write to pr
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 20:08:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6508" class=".btn">#6508</a>
            </td>
            <td>
                <b>
                    Test that peers are not disconnected in `RetryingSwitchingPeerMessageTaskTest::failsWhenAllPeersFail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Check that since we are below the max number of peers, no peer should be disconnected

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

relates to  #6465
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 13:49:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6505" class=".btn">#6505</a>
            </td>
            <td>
                <b>
                    Code storage by hash v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This is a redo of https://github.com/hyperledger/besu/pull/5889 including a fix for detection of existing storage.

---

Storing code by hash instead of by address. This is needed so that Besu can serve snapsync as we need to be able to retrieve the code by hash.

After syncing with this change it's not possible to downgrade to an older version of Besu. If we think this is needed I could add a subcommand to do the conversion.

**Testing**
- Checkpoint sync on Sepolia, Goerli and Mainnet
- Confirmed the same code bytes were stored for both column families by running a comparison tool on the stored code bytes https://github.com/hyperledger/besu/pull/6019/files#diff-9c4d660b9f0b067bbaf230c40ff79f2a53fef78e88c0c5e368b43e3891d0f68bR227
- Compatibility testing to ensure that existing databases continue to work
- Compared storage of code size on mainnet. Before: 9 GiB After: 2GiB. Column family to store code counts i.e. `CODE_HASH_COUNT` is using 38 MiB.
- Compared FCU and new payload times on mainnet with and without code changes showing no significant difference in times
<img width="2483" alt="Screenshot 2023-10-16 at 10 07 15 am" src="https://github.com/hyperledger/besu/assets/909467/ef6f5b7a-26f1-4831-94c9-a5397d04f53b">
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 07:27:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6504" class=".btn">#6504</a>
            </td>
            <td>
                <b>
                    Revert "Bonsai code storage by hash (#5889)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 9c02518f012deb2c20a5551973e556df09d9c930.

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Found a bug during additional testing see https://github.com/hyperledger/besu/pull/6502. Out of caution reverting the change so that it doesn't cause an issue using this feature. 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 06:42:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6501" class=".btn">#6501</a>
            </td>
            <td>
                <b>
                    Deprecate --Xp2p-peer-lower-bound
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Deprecate CLI option --Xp2p-peer-lower-bound and remove usage

Fixes #6376
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 03:46:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6500" class=".btn">#6500</a>
            </td>
            <td>
                <b>
                    [MINOR] remove duplicate setting of default values for CLI options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                where the default is number/boolean/string, just leave it to the initialized value for the actual field.

same as was done for Sync Options in #6499
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:44:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6499" class=".btn">#6499</a>
            </td>
            <td>
                <b>
                    Flat db heal - deprecate CLI option and set to always true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * set flat db healing enabled to true always
* remove duplicate setup of default values from Sync Options class

refs #6157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:26:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6498" class=".btn">#6498</a>
            </td>
            <td>
                <b>
                    Filter Discovered peers for ipv6 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
updates PeerDiscoveryAgent to 
* use existing NetworkUtility to filter for any/none peers
* fall back to source address if ipv6 is not supported (like in a docker container)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #6475 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 01:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6496" class=".btn">#6496</a>
            </td>
            <td>
                <b>
                    [Refactor] Move graphqloptions to its own class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Move GraphQl options options to its own class

## Fixed Issue(s)
see https://github.com/hyperledger/besu/issues/6428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-30 21:46:25 +0000 UTC
    </div>
</div>

