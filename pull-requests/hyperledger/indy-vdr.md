---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/86" class=".btn">#86</a>
            </td>
            <td>
                <b>
                    Feature/proxy with multiple ledger support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Indy Vdr Proxy with multiple ledger support and DID Resolution API (based on Indy Vdr's `PoolResolver`)
- Refresh (after initial refresh) is not yet working.
- I've included a dockerfile for a node-pool based on Indicio's indy-node branch with the did:indy implementation  (HT @dbluhm). This pool is now used for the integration tests in indy-vdr's did-indy branch.

## Usage

The `indy-vdr-proxy` executable can be used to provide a simple REST API for interacting with one or more Indy ledgers. Command line options can be inspected by running `indy-vdr-proxy --help`.

To start the proxy server for a single ledger use the following command:
`indy-vdr-proxy -p <PORT> (-g <OPTIONAL_PATH_TO_GENESIS_FILE>)`

To start the proxy server with the standard configuration of indy ledgers use the following command:
`indy-vdr-proxy -p <PORT> --multiple-ledgers`
This will get the ledger configuration from `https://github.com/IDunion/indy-did-networks`

A custom ledger configuration can be provided either by specificing a Github repo or a local folder:
`indy-vdr-proxy -p <PORT> --multiple-ledgers -g <GITHUB_URL or PATH_TO_FOLDER>`
The structure needs to be as follows `<NAMESPACE>/OPTIONAL<SUB_NAMESPACE>/pool_transactions_genesis.json`, e.g. `/sovrin/staging/pool_transactions_genesis.json`

Responses can be formatted in either HTML or JSON formats. HTML formatting is selected when the `text/html` content type is requested according to the Accept header (as sent by web browsers) or the request query string is set to `?html`. JSON formatting is selected otherwise, and may be explitly selected by using the query string `?raw`. For most ledger requests, JSON responses include information regarding which nodes were contacted is returned in the `X-Requests` header.

Sending prepared requests to the ledger is performed by delivering a POST request to the `{LEDGER}/submit` endpoint, where the body of the request is the JSON-formatted payload. Additional endpoints are provided as shortcuts for ledger read transactions:

- `{LEDGER}/` The root path shows basic status information about the server and the ledger pool
- `{LEDGER}/genesis` Return the current set of genesis transactions
- `{LEDGER}/taa` Fetch the current ledger Transaction Author Agreement
- `{LEDGER}/aml` Fetch the current ledger Acceptance Methods List (for the TAA)
- `{LEDGER}/nym/{DID}` Fetch the NYM transaction associated with an unqualified DID
- `{LEDGER}/attrib/{DID}/endpoint` Fetch the registered endpoint for an unqualified DID
- `{LEDGER}/schema/{SCHEMA_ID}` Fetch a schema by its identifier
- `{LEDGER}/cred_def/{CRED_DEF_ID}` Fetch a credential definition by its identifier
- `{LEDGER}/rev_reg/{REV_REG_ID}` Fetch a revocation registry by its identifier
- `{LEDGER}/rev_reg_def/{REV_REG_ID}` Fetch a revocation registry definition by its registry identifier
- `{LEDGER}/rev_reg_delta/{REV_REG_ID}` Fetch a revocation registry delta by its registry identifier
- `{LEDGER}/auth` Fetch all AUTH rules for the ledger
- `{LEDGER}/auth/{TXN_TYPE}/{ADD|EDIT}` Fetch the AUTH rule for a specific transaction type and action
- `{LEDGER}/txn/{SUBLEDGER}/{SEQ_NO}` Fetch a specific transaction by subledger identifier (0-2, or one of `pool`, `domain`, or `config`) and sequence number.

If the proxy server is used with a single ledger, the `{LEDGER}` part of the path must be omitted.

### DID:Indy Resolver

Indy VDR contains a DID Resolver to resolve DIDs and dereference DID Urls to ledger objects from configured ledgers according to the [did:indy specification](https://hyperledger.github.io/indy-did-method/).

`GET /1.0/identifiers/{DID or DID_URL}`



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 16:58:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Feature/general indy resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Builds upon #80 

- Adds a VDR API with a general DID resolver. Network configuration can be taken from a Github Repo or a local folder structure
- Initial support for multiple ledgers and DID resolution with indy-vdr-proxy

The VDR API uses Async/Await and is therefore not suited for FFI, but I'll look into it.

I think it would help to create a `did-indy` branch to have smaller PRs at some point :) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 16:32:52 +0000 UTC
    </div>
</div>

