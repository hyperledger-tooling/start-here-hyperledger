---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2630" class=".btn">#2630</a>
            </td>
            <td>
                <b>
                    Feature Suggestion: Include a Reason When Constraints Cannot Be Applied
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When the verifier agent is unable to apply a constraint filter, it would be helpful for the Problem Report to include a reason why it failed. For example, instead of:

```
Constraint specified for input_descriptor_123 does not apply to the enclosed credential in $.verifiableCredential[0]
```

... the message could include the reason that the constraint could not be applied, with the specific path or item that did not match. For example:

```
Constraint specified for input_descriptor_123 does not apply to the enclosed credential in $.verifiableCredential[0]
Reason: Credential is not applicable for field 11111111-2222-3333-4444-56789abcdef0 with paths ['$.credentialSubject.part1.part2']
```

This indicates that the field indicated in the message was not found in the Reveal Document or the full Credential.

or

```
Constraint specified for input_descriptor_123 does not apply to the enclosed credential in $.verifiableCredential[0]
Reason: No field in constraints for part2 under parent path "$.credentialSubject.part1"
```

This indicates that the "part2" property found in the Reveal Document under "$.credentialSubject.part1" was not found in the list of fields in the constraints.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 22:22:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2629" class=".btn">#2629</a>
            </td>
            <td>
                <b>
                    Update the ReadTheDocs config in case we do another 0.10.x release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This file has not been updated for the last two releases, and as such, the ReadTheDocs deployments have not worked. Not the end of the world, but adding this file now in case we do another release, and I forget again. If we don't do another deploy -- no harm done.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 18:52:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2627" class=".btn">#2627</a>
            </td>
            <td>
                <b>
                    0.11.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 0.11.0 release -- including adding the CHANGELOG entries for releases 0.10.2 - 0.10.5 to the main branch CHANGELOG.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 23:06:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2626" class=".btn">#2626</a>
            </td>
            <td>
                <b>
                    chore: bump pydid version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After the recent removal of peer-did-python in #2561, pydid no longer needs to be pinned below 0.4.x. This PR bumps the version to ^0.4.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-24 16:36:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2623" class=".btn">#2623</a>
            </td>
            <td>
                <b>
                    0.10.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 22:54:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2622" class=".btn">#2622</a>
            </td>
            <td>
                <b>
                    fix(backport): report presentation result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a backport of #2615 for the 0.10.x branch of releases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 21:23:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2618" class=".btn">#2618</a>
            </td>
            <td>
                <b>
                    fix: wallet type help text out of date
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2617 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 05:28:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2615" class=".btn">#2615</a>
            </td>
            <td>
                <b>
                    fix: report presentation result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR ensures that the result of verifying the presentation for JSON-LD Credentials is factored into the final `verified` status.

cc @andrewwhitehead  @swcurran 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 18:20:39 +0000 UTC
    </div>
</div>

