---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    File key regex case insensitive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 19:54:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Add CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 14:37:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Bug Fix and Other Enhancements to CA Support for mTLS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Fixes

Originally p2p APIs were using `req.client.getPeerCertificate().issuer` to determine the ID of the DX which sent the request. This worked for self-signed certificates because the `issuer == subject`, however for CA-signed certs provisioned w/ cert-manger, or internal Kaleido certs signed with a environment's CA, the `issuer != subject` and it was causing issues with private messaging E2E tests in those environments. `subject` should be used because DX uses it to derive its own peer ID that it advertises on `GET /id`.

For example, w/ a cert-manager cert signed by a CA (the CA happened to not have an O or OU) the DX would get the following error when trying to hit another org's DX:

```
2021-07-14T16:54:18.679Z [ERROR]: post https://a-firefly-host/api/v1/messages attempt 0 [500] { error: 'Invalid peer' } utils.ts
```

By casting the socket of the req to the `TLSSocket` it allows Typescript to then retrieve the `subject` from the peer's certificate which is what should be used to derive the DX's ID from the O and OU.

## Additions

With cert-manager certificates, the `cert.pem` does not include the CA which signed it. If the CA is self-signed, this needs to be advertised in `GET /id` so peers can include the CA in their `HttpsAgent` and when they persist the certs in the `peer-certs` directory.

This adds support to _optionally_ (if the file exists) read a `ca.pem` file from the `DATA_DIRECTORY` (same directory as `key.pem` and `cert.pem`) and prepend it the `cert.pem` storing it in a new var `certBundle`. `certBundle` is then returned on `GET /id` so peers will receive both the cert and the provided CA. The `cert` var is left to only contain the `cert.pem` because including the CA seemed to break the server startup when used in the `TLSContext`.

While self-signed CAs were already supported by putting a `ca.pem` in the `peer-certs` directory before startup (as what was is currently documented in the README) this _allows peers to have certs signed by separate CAs_ w/o every peer needing to be aware of them on startup. It also allows new DX peers to join the network with renewed CA certs.

## Original Issue

These changes arose from issues we found w/ FF DX deployments using self-signed CAs where the NodeJS HTTPS agent couldn't trust the cert from a peer bc the CA wasn't included in the chain (in a lot of ways this was just a config issue):

```
2021-07-14T15:23:19.854Z [ERROR]: post https://a-firefly-host/api/v1/messages attempt 2 [undefined] Error: unable to verify the first certificate
    at TLSSocket.onConnectSecure (_tls_wrap.js:1514:34)
    at TLSSocket.emit (events.js:375:28)
    at TLSSocket._finishInit (_tls_wrap.js:936:8)
    at TLSWrap.ssl.onhandshakedone
```

However, in Kubernetes environments where `peer-certs` is backed by a PVC, the `ca.pem` cannot be included into the directory before startup without init/bootstrap scripts (for example see the [Helm chart PR in firefly](https://github.com/hyperledger-labs/firefly/pull/114/files#diff-abf2c3ec729c16f0ff294d8b85ac9fa0c5a747bc602839b95fd4040466f829b5R68-R84)). Upon adding the `ca.pem` / `certBundle` feature the bug above around the `subject` of the peer certificate was then discovered and needed to be fixed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 17:06:49 +0000 UTC
    </div>
</div>

