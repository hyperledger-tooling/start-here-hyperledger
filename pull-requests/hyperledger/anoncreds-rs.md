---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    chore: update versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 12:19:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/131" class=".btn">#131</a>
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
                Similar to https://github.com/hyperledger/indy-vdr/pull/170 and https://github.com/hyperledger/aries-askar/pull/111 but for anoncreds


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 13:45:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    fix(js): missing getXXXFromJson methods and several typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding the missing methods from react-native wrappers and making lots of minor fixes, mostly related to typos and outdated variable/method names.

At the moment working for a full issuance / present proof / verify proof flow without revocation (yes, also possible to issue a credential in React Native 🎉). However there is a memory leak leading to custom app crashes and variable corruption (!) when creating presentation.  Based on some debugging I did, the corrupted variables are strings in some FFI lists: it seems that strings are cleared or updated by the runtime before they are used by native library. Not sure if this makes sense, but I noticed that if I use short strings for fields like `issuerId`, `schemaId` and `credentialDefinitionId` (e.g. _'mock:uri'_) the flow works fine consistently, while if I use relatively long strings (real full DIDs, 50 characters long or so, no matter if it's only one of these variables), the flow crashes almost always. 🤔 

Also I think in some methods (like the aforementioned `createPresentation`) we are missing data deallocation but not completely sure how to handle that yet (@blu3beri you have all lottery numbers for this prize!! 😄). Work done in #129 will certainly help but I don't think if it's enough in a long-term app session. 

PS: All getXXXFromJson methods can be heavily refactored as they do almost the same thing. For the moment just wanted to be conservative to be focused in solving all issues, but any suggestion to make it cleaner will be appreciated!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-05 10:46:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    refactor(js)!: use JSON objects in API instead of strings and instances
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an attempt (without doing anything revolutionary) to make JS API a bit more simple to use, avoiding the so-many conversions from JSON to string  that we found during integration with AFJ. 

For most methods that are currently receiving `AnoncredsObject` instances, now we accept also passing JSON objects. This makes the caller to not care about object instantiation and clearing handles, which is done internally. Hopefully, in a normal flow the caller will need only to care about freeing a few objects (like Credentials).

I'm not sure if I'm using the `try-finally` method correctly (I'm particularly worried about the order of execution of finally if an exception is thrown) so any comments on this approach would be appreciated. I wanted to make this process of "checking object type and loading from JSON/add to handles to clear array" more elegant, but I think I'll need some more TypeScript lessons from @TimoGlastra and @blu3beri before attempting to do that 😛 .

Some tests were added to this repo, but I didn't check this as a patch of AFJ to see how is it going, something I'd like to do before merging. 

Summary of changes: 

- Refactor `load` in AnonCredsObjects to `fromJson`, loading from a JSON object rather than a string
- Refactor `toJson` in AnoncredsObject to return a JSON object rather than a string
- All constructors and methods in API AnoncredsObjects accept both AnonCredsObjects and JSON objects. This is the most tricky part: for every passed JSON object, an  ephemeral AnonCredsObject instance will be created and must be cleared before returning to the caller
- Add some missing fromJson (like the one from Credential)
- Rename keyProof -> keyCorrectnessProof to match the naming of other fields

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 19:01:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    update `ursa` to 0.3.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `ursa` version 0.3.6 still has dependencies on the long deprecated `failure` crate which is no longer maintained and contains well known security issues (CVE-2019-25010 and CVE-2020-25575).

fix #123 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 10:38:34 +0000 UTC
    </div>
</div>

