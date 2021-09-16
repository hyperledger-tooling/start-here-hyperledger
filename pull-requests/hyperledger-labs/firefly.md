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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Gracefully shutdown http server when resetting config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hopefully this should fix https://github.com/hyperledger-labs/firefly-cli/issues/80

The behavior in that issue has been very difficult to reproduce, but this code should help. Even if it doesn't fix that issue, it will not hurt anything else, and it helps prevent other http requests from possibly getting interrupted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 14:09:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    bump ui to version 0.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ♾️ 📜 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 18:44:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    Add architecture videos to docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the relevant community call architecture discussions to their respective pages on the docs site.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 17:53:16 +0000 UTC
    </div>
</div>

