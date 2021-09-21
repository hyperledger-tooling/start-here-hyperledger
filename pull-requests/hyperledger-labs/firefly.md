---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Replace operation "info" with separate "input" and "output" fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Existing field has evolved to always contain plugin-specific data generated upon
completion of the operation. There is also a (separate) use case for storing
input data upon creating the operation, to support e.g. retryability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 16:38:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Factor out "PersistTransaction" as a common database utility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No idea where would be the appropriate place for this... but this general logic of validating and marking
a transaction complete is going to be needed outside of `events` (specifically, tokens look to be
introducing a new type of transaction that will be marked complete by a call in `syshandler`).

This logic is all transaction- and database-related (not particularly related to events). It's also not
particular to a specific database (ie SQL), although some of the checks could be pushed down into
the SQLCommon handler. Looking for input on whether a common utility like this is a good idea, or
if there's a better way to handle this common logic across packages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 16:05:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    Small fixes to token accounts
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
        Created At 2021-09-16 20:19:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Add identity manager and API input matrix logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work in progress on https://github.com/hyperledger-labs/firefly/issues/187

Key proposals in this code so far - building with Unit Tests
- New `Identity Manager [Im]` component
   - This is _not_ a plugin, instead a consistent component to do all identity mapping
   - This would be expected to be where plugins would attach in the future
   - Implementation includes testing of the various matrix options
   - Implementation includes wiring this into `Orchestrator`
   - Implementation includes changing imports on calling packages
   - TODO (in this PR): Fix all the code that that currently calls `Resolve` on the now defunct Identity Interface
- New `fftypes.Identity` sub-object
   - Intended to replace single `author` field with `author`+`key` fields
   - Pass pointer to this part of the struct to the new `im.ResolveInputIdentity` function
   - TODO (in this PR): Embed this into all objects that can contain identity
- Stubbing out the `Identity Interface [Ii]` plugin for now
  - Still retained `onchain` key for config compatibility
  - Removed all methods from interface
  - Changed implementation to `TBD` for now in the code
 - Organizations and Nodes still use the signing identity
  - For now the intention is that `Node.Owner` and `Organization.Identity` remain the signing addresses
  - We should move these to be DIDs, but that will mean migration issues
   - Per https://github.com/hyperledger-labs/firefly/issues/187#issuecomment-919649333 we need to consider this before acting

The next step here is e2e testing, and working through various scenarios to test.
I have only done build+UT so far.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 05:41:23 +0000 UTC
    </div>
</div>

