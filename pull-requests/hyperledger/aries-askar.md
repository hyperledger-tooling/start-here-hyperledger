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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    fix(js): empty key entry list metadata in react-native
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This prevents a crash  when fetching an existing key in iOS (and likely also in Android) and `askar_key_entry_list_get_metadata` returns NULL:

![image](https://user-images.githubusercontent.com/4800462/221714690-915db1cd-6f8b-43c1-b065-375bce0efdb7.png)

Not sure if the same should be applied to other parts of the code (it was already done in some other methods such as `entryListGetTags` and  `keyEntryListGetTags`).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 23:46:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    feat: migration pre-upgrade script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I added the [migration but not the conversion](https://github.com/hyperledger/aries-acapy-wallet-upgrade/blob/6494f068278d85accde2d066bc26f162489f5b57/acapy_wallet_upgrade/strategies.py#L745-L750) script to aries-askar itself. 

It is added as a feature (default right now, but can be removed). After a while we can probably remove it from the default features as most people have migrated, but then it can always be opted-in of course.

I was working on the migration script for React Native Sqlite wallets and I was running into a lof of issues regarding sqlite and cryptography dependencies. Every sqlite dependency came with a list of issues and it since we can not patch them (as the sqlite dependency has to be a direct dependency of the wallet), it seemed unfeasible.

I tried to depend on the values / structs / functions from aries-askar itself as much as possible, but I might have created some duplicate code. @andrewwhitehead you can probably spot this a lot better than me here.

The python script could also depend on this function, but it is not required.

The script also only supports indy-sdk sqlite -> aries-askar sqlite. There is no additional support for multiple wallets (although the script can be be called multiple times for this to work, however untested). Postgres has been omitted for now as it did not fit the direct use case. I don't think that adding support for Postgres would be all too complex.

Curious to hear if there are any objections to this PR or if there is a very specific reason why it was not done for the Python script.

cc: @TimoGlastra @andrewwhitehead @swcurran 

NOTE: It does not really have a test, yet. I would have to create an indy-sdk wallet and I am not too sure what the quickest way is to do that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 13:53:52 +0000 UTC
    </div>
</div>

