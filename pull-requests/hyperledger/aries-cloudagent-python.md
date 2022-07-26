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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1870" class=".btn">#1870</a>
            </td>
            <td>
                <b>
                    Indy ledger fixes and cleanups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Move `check_existing_schema `, `create_and_send_schema` and `create_and_send_credential_definition` to the `BaseLedger` class, to avoid duplication between `IndySdkLedger` and `IndyVdrLedger` backends
- Fixes a logic error in `create_and_send_credential_definition` in `IndyVdrLedger`
- Remove unnecessary session creation in `IndySdkLedger`

I think this should resolve the most common integration test failures (published cred def not found in wallet).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 18:43:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1866" class=".btn">#1866</a>
            </td>
            <td>
                <b>
                    feat: add universal resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR merges the universal resolver plugin into main ACA-Py. This PR adds a couple new CLI args to configure usage of the universal resolver.

By default, the universal resolver is NOT loaded. If the `--universal-resolver` flag is given, without arguments, it will default to using `https://dev.uniresolver.io` for convenience. We might want to add language somewhere discouraging people from using this endpoint all the time. We should encourage people to use `--universal-resolver https://my.universal.resolver.com` to point to their own deployed universal resolver instance.

By default, if the resolver is loaded, it will retrieve properties from the universal resolver and use that to compile a regex that matches all supported DIDs. This regex will be used to determine if a given DID is supported by the resolver. Alternatively, the user can specify `--universal-resolver-regex regex-one regex-two regex-three` to manually configure what DIDs should be supported by the universal resolver. This is useful when you want to limit usage of the universal resolver to a known "trustworthy" set of DIDs or similar. The arguments to `--universal-resolver-regex` are compiled into a single regex on startup.

cc @swcurran 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 18:35:15 +0000 UTC
    </div>
</div>

