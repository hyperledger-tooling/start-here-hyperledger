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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2491" class=".btn">#2491</a>
            </td>
            <td>
                <b>
                    Update steps for Manually Creating Revocation Registries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add critical missing step.

------------

This PR addresses an issue with the documentation discovered here; https://github.com/bcgov/DITP-DevOps/issues/109#issuecomment-1713894110
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 14:11:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2490" class=".btn">#2490</a>
            </td>
            <td>
                <b>
                    Issue #2488 KeyError raised when Subject ID is not a URI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed from `value`, which may or may not be a list, to `subject`, derived from `subjects` which is always a list.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 06:03:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2487" class=".btn">#2487</a>
            </td>
            <td>
                <b>
                    Feat/sd jwt implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds SD-JWT support for sign and verify endpoints, including optional key binding.

By default, all claims at all levels of the payload can be selectively disclosable (with the exception of essential verification data such as iss, iat, cnf, etc.), unless indicated otherwise by the issuer.

Info from @dbluhm: This PR, like the JWT sign and verify endpoints added previously, adds basic support for creation and verification of SD-JWTs. The methods/endpoints do not place any expectations on the payload beyond those required by the SD-JWT specification; in other words, the payload is not required to be a VC. As it stands, this enables other services to take advantage of ACA-Py's secure storage and DID Resolution capabilities to create and verify SD-JWT VCs but does not enable ACA-Py to do the same on its own. This is the foundational work required to later add support for SD-JWT VCs to the rest of ACA-Py's Issuance and Verification stacks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 21:40:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2486" class=".btn">#2486</a>
            </td>
            <td>
                <b>
                    Feat: Upgrade from tags and fix issue with legacy IssuerRevRegRecords [<=`v0.5.2`]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2485 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 20:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2484" class=".btn">#2484</a>
            </td>
            <td>
                <b>
                    0.10.2
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
        Created At 2023-09-08 00:37:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2483" class=".btn">#2483</a>
            </td>
            <td>
                <b>
                    Update devcontainer to read version from aries-cloudagent package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update sample files and documentation for ruff usage.

The main purpose of the PR is to address changes in version from #2471.

See an ill-advised workaround at #2481 for more reference. Main issue is running the pytests in the devcontainer. Thanks @dbluhm for questioning if that PR was the right thing to do (it wasn't).

This also updates `flake8` references in devcontainer to `ruff` and updates example run configs.

Closes #2455 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 20:01:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2482" class=".btn">#2482</a>
            </td>
            <td>
                <b>
                    0.10.2 Patch Release - fix issue #2475, #2477
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Re 0.10.2-rc0 patch release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 18:31:21 +0000 UTC
    </div>
</div>

