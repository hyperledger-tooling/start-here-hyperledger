---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    Restrict default max conns to a range for sqlite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now using a default maximum number of connections between 2 and 8 even when the detected number of CPUs is higher or lower.

Related: #109 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 17:39:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    chore: update version to dev.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the version to dev.4. 

We want to wait for a release until #111, #104, #108 & #89 are merged (which are mostly waiting for the broken CI)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 13:25:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    fix(js): several fixes for js wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains several fixes from integrating aries askar into react native. 

Mainly it resolves:
- https://github.com/hyperledger/aries-askar/issues/77
- incorrect creation of errors in React Native (no AriesAskarError, but string)
- null pointer handling

Draft as it still needs to be tested fully in React Native
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 12:23:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    fix(js): ensure scan is freed after fetchAll
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When using `Scan.fetchAll` I found that the scan handle was not always properly freed. It turns out that this had to do with an error thrown when calling `scanNext` due to no records have been found (related issue https://github.com/hyperledger/aries-askar/issues/77), which prevented the code from executing the scanFree call.

So here we simply add a try-finally to make sure it is always being called.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-04 01:20:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    fix(js): free key and entry objects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As there is not a destructor in JS, objects must be freed manually. This PR attempts to free any native object after it is used, making life easier to consumer applications. 

If this approach is correct, the only objects an app using this library should care about is `Key` (for which I added the missing call to `keyFree`).

@blu3beri let me know if concepts applied here are correct so I can replicate for anoncreds-rs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 02:39:37 +0000 UTC
    </div>
</div>

