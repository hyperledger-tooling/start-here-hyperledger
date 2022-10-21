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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1984" class=".btn">#1984</a>
            </td>
            <td>
                <b>
                    Additional 0.7.5 Cherry-Pick
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contains the following PRs:
- [x] https://github.com/hyperledger/aries-cloudagent-python/pull/1938
- [x] https://github.com/hyperledger/aries-cloudagent-python/pull/1926
- [x] https://github.com/hyperledger/aries-cloudagent-python/pull/1973

Reference issue #1983 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 16:41:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1982" class=".btn">#1982</a>
            </td>
            <td>
                <b>
                    Fixed bug in run_demo script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed a bug which prompts out when we try to use the debugging capabilities inside the demo.
The command:
```
LEDGER_URL=http://dev.greenlight.bcovrin.vonx.io ./run_demo alice --events --no-auto --debug-pycharm-controller-port 5003 --debug-pycharm-agent-port 5004 --debug-pycharm --wallet-type indy
```
was failing in attaching the debug servers without such fix. Now it works.

It applies also for `faber` and `acme` instances.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 17:04:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1981" class=".btn">#1981</a>
            </td>
            <td>
                <b>
                    feat: update pynacl version from 1.4.0 to 1.50
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this fixes install for m1 mac arm64 arch

closes #1980 

Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 13:29:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1978" class=".btn">#1978</a>
            </td>
            <td>
                <b>
                    chore: fix ACAPY_PROMOTE-AUTHOR-DID flag 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                using underscore instead of hyphen

closes #1965 

Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 13:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1977" class=".btn">#1977</a>
            </td>
            <td>
                <b>
                    fix: public did mediator routing keys as did keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes an issue @reflectivedevelopment found while using the recent changes made to support routing keys associated with public DID endpoints.

Without this fix, when creating a public DID OOB invitation, creation will fail due to no DIDComm service being found. This stemmed from PyDID expecting that routing keys be expressed strictly as DID URLs. Previously, we were resolving the routing keys as raw base58 encoded public keys. This PR makes it so that routing keys are resolved as did:key url values (if already did:key, simply pass through the values but if not, transform into did:key urls).

Credit to @cjhowland for doing most of the digging on this issue :slightly_smiling_face: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 18:52:24 +0000 UTC
    </div>
</div>

