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
                PR <a href="https://github.com/hyperledger/aries-askar/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Support for Swift wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes #99, which is necessary for Swift.

The xcframework built for reactive-native can be shared with the Swift wrapper. But, it requires a different archive format. So I added a workflow step to archive it using `zip` with a different folder name `AskarFramework`.
The Swift wrapper in different repo could download the zipped xcframework for its dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 07:20:28 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Update version to 0.2.8
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
        Created At 2023-03-01 23:39:02 +0000 UTC
    </div>
</div>

