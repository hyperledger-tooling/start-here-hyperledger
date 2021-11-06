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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/378" class=".btn">#378</a>
            </td>
            <td>
                <b>
                    Make thread id optional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 11:00:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    Add code of conduct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 10:08:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/376" class=".btn">#376</a>
            </td>
            <td>
                <b>
                    Simplify issuer offer sending API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span><span class="chip">breaking</span>
            </td>
            <td>
                Before, credential offer was sent in e.g. NodeJS as follows:
```
    const issuerCred = await IssuerCredential.create({
      attr,
      sourceId: 'alice_degree',
      credDefHandle,
      credentialName: 'cred',
      price: '0',
      issuerDid
    })
    await issuerCred.sendOffer(connection)
```
In order to simplify the API (and the internal code), this was changed to (again, using NodeJS only as an example):
```
    const issuerCred = await IssuerCredential.create('alice_degree')
    logger.info(`Per issuer credential ${issuerCredId}, sending cred offer to connection ${connectionId}`)
    await issuerCred.sendOffer(connection, {
      attr,
      credDefHandle
    })

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 15:36:22 +0000 UTC
    </div>
</div>

