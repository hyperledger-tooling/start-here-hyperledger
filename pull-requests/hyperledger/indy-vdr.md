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
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Changes for did:indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a WiP pull request for changes relating to did:indy

- [x] Adds new properties to `NymOperation`  (`diddocContent`)
- [ ] Adds new properties to `GetNymOperation`  (`seqNo`, `timestamp`)
- [x] Adds resolver module to resolve ledger objects according to  did:indy spec

## Resolver
The resolver is initialized per pool/ledger ([example](https://github.com/IDunion/indy-did-resolver/blob/e2d7d1971006ecc6a124b0be1febd2fed9270f8e/indy-did-driver/src/main.rs#L49))

## Backward compatibility

As mentioned in #74, I don't really know what's the best way to handle backward compatibility.
I've implemented one possibility for the `NymOperation`, i.e. the `build_nym_request` function in particular.
I've introduced two new functions `build_nym_request_did_indy` and `build_nym_request_legacy`. The former accepts the additional, optional `diddoc_content` parameter. Depending on the feature flag `legacy`, either  `build_nym_request_did_indy` or `build_nym_request_legacy` gets exposed as `build_nym_request`.
I'm totally not sure if this is a reasonable approach :)

## Proxy

Ideally, the proxy would expose the resolver as an  API compatible with the universal resolver. Currently, the proxy manages only a single pool/ledger. We'd need to change the proxy to manage multiple pools/ledgers.

## Wrapper

How do we change the wrappers with respect to backward compatibility?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-21 14:39:08 +0000 UTC
    </div>
</div>

