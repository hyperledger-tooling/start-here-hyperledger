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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2950" class=".btn">#2950</a>
            </td>
            <td>
                <b>
                    CodeCov report on PR's
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will bring back `codecov` reporting on PR's and add comments like:

![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/1d4c9db8-a5af-4ec0-9c90-8ef8248b9040)

The warning only happened because I forced pushed.

The readme badge should also start working again.

There is a bit of setup for the repo admin. I'm hoping the covecov account that was used a year ago can be used again. The repo admin has to setup a token. It's really easy. The instructions are here https://docs.codecov.com/docs/github-2-getting-a-codecov-account-and-uploading-coverage.

Note: The unit tests for this PR won't pass until the token is available. 
![image](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/ab6fa794-396c-4d5c-8f72-75ed65a25799)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 21:52:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2948" class=".btn">#2948</a>
            </td>
            <td>
                <b>
                    Example integration test issuing 2 credentials under the same schema
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
        Created At 2024-05-14 17:34:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2947" class=".btn">#2947</a>
            </td>
            <td>
                <b>
                    DOC: Verifiable Credential Data Integrity (VC-DI) Credentials in Aries Cloud Agent Python (ACA-Py)
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
        Created At 2024-05-14 08:08:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2946" class=".btn">#2946</a>
            </td>
            <td>
                <b>
                    Anoncreds - Send full registry list when getting revocation states
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.0.0</span>
            </td>
            <td>
                See https://github.com/hyperledger/aries-cloudagent-python/issues/2934.

So this ended up being a one line fix. The anoncreds legacy_indy implementation for the holder, was getting the revocation list (registry) from the ledger. Then it was removing index 0, which doesn't actually represent a credential but is expected by anoncreds-rs when getting the revocation state. See https://github.com/hyperledger/anoncreds-rs/issues/336.

This is a bit weird and will need to be remembered when other implementations get added.

I have tested with the demo and manually. I still want to make an integration test for this scenario.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 21:33:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2945" class=".btn">#2945</a>
            </td>
            <td>
                <b>
                    chore: updating dependabot to support gha, python, docker and dev container packages
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
        Created At 2024-05-10 16:21:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2943" class=".btn">#2943</a>
            </td>
            <td>
                <b>
                    fix(interop): overly strict validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.0.0</span>
            </td>
            <td>
                This change relaxes some overly strict validation that was preventing presenting proof using LDP-VC from Credo 0.5.X based agents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 00:28:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2940" class=".btn">#2940</a>
            </td>
            <td>
                <b>
                    :arrow_up: Upgrade lint dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.0.0</span>
            </td>
            <td>
                ⬆️ Upgrades:

- `black`: 24.3.0 -> 24.4.2
- `ruff`: 0.1.2 -> 0.4.4
- `pre-commit`: 3.3.3 -> 3.7.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 18:45:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2939" class=".btn">#2939</a>
            </td>
            <td>
                <b>
                    :arrow_up: Upgrade test dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.0.0</span>
            </td>
            <td>
                :arrow_up: Upgrades:
- `pytest`: 8.0.0 -> 8.2.0
- `pytest-asyncio`: 0.23.5 -> 0.23.6
- `pytest-cov`: 4.1.0 -> 5.0.0
- `pytest-ruff`: 0.1.1 -> 0.3.2

➖ Removes:
- `mock`
  - This dependency is used to provide unittest.mock features to older version of python
  - Not needed with current python version

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 18:28:24 +0000 UTC
    </div>
</div>

