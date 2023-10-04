---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1008" class=".btn">#1008</a>
            </td>
            <td>
                <b>
                    Do not test/build vdrtools anoncreds in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Dont test/build vdrtools anoncreds in CI
- Change aries-vcx default features from `vdrtools` to `modular`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 14:46:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1007" class=".btn">#1007</a>
            </td>
            <td>
                <b>
                    Use a sequence of bytes (representing AriesMessage) as input for EncryptionEnvelope::create
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
This makes it more general, allowing use of the utility methods without worrying about the exact structure of `AriesMessage` passed in. In doing so, allows for also wrapping message types not yet recognized in aries_vcx.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 12:30:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1006" class=".btn">#1006</a>
            </td>
            <td>
                <b>
                    Do not delete target wallet, do not fail migration on item-error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is set of changes to make the migration.
- More graceful, one migration error should not halt migration of the rest. It's up to migrating user to evaluate whether the migration result is satisfactory.
- Idempotent - if migration fails for example due an IO error midway, it should be possible to finish it on 2nd try.

Changes:
- If migration fails, do not delete the target wallet.
- Disable adding records to vdrtool cache when running migration.
- Do not fail migration if the record has unexpected format. Just skip it and log the record. 
- If migration of the record itself fail, skip it and log.
- If adding item to target wallet fails due duplication error, skip it. For idempotency it would be ideal to overwrite it, but that would need digging deeper. For now, skipping these records still gives us idempotency under assumption item migration process was not changed between 2 migrations attempts.
- If adding item fails for other reason, fail the migration (likely IO error).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 06:45:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1005" class=".btn">#1005</a>
            </td>
            <td>
                <b>
                    Refactor/remove mocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are plenty of occurrences where some occult mocking mechanism is employed by holding some global settings `HashMap` and setting/getting values from it.

This PR explores and aims to deal with this in multiple ways:
- remove this completely if possible
- adjust the mocks to only be employed when testing through `#[cfg(test)]`

This sets the ground for better decoupling the test code from production code which might even be done to some extent within this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 09:15:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1004" class=".btn">#1004</a>
            </td>
            <td>
                <b>
                    Add logs to credx wallet migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add logs to credx migration
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-01 17:56:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    Use generics over trait objects in Profile & co.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A valiant attempt at relying more on generics rather than the `Arc<dyn>` madness. 

Unfortunately, these have become so deeply rooted within some crates that it's pretty hard to do it incrementally. There's also pretty much no data flow to follow because everything was `Arc`'ed and cloned in a lot of places effectively bypassing the ownership model of Rust.

`libvcx` was worked around by some generic implementation on the traits over the `Arc<dyn>` stuff. If you ever wondered whether some code can make a grown man cry, I'll answer that for you. Yes. Yes it can.

Ideally the components ownership should be established and refactors should be done to make it clear what gets used where and why. This however will span across tests, the primitives traits and a lot of production code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 09:39:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1002" class=".btn">#1002</a>
            </td>
            <td>
                <b>
                    Use standard UnpackMessageOutput struct until finally needing to transform.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As [suggested in](https://github.com/hyperledger/aries-vcx/pull/992#discussion_r1337239159) review of #992 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 14:26:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    Move CI dir
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moved the `ci` directory under `.github` and cleared out some remaining items from previous Java/iOS wrappers in some scripts. Obsolete `rustfmt.toml` files were also removed (which lead to a lot of files being formatted).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 09:19:10 +0000 UTC
    </div>
</div>

