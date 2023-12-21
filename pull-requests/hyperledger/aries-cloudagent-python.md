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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2687" class=".btn">#2687</a>
            </td>
            <td>
                <b>
                    Emit did:peer:2 for didexchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rather than manage repo permissions. I'm reopening @dbluhm 's [PR](https://github.com/hyperledger/aries-cloudagent-python/pull/2578) here so I can verify and add/restore tests. 

- [x] Restore Unittests
- [ ] Restore integration tests
- [ ] Add new unit tests
- [ ] Add new integration tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 22:13:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2686" class=".btn">#2686</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This brings in indy-vdr 0.4.1, with better performance on pool refreshes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 21:51:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2684" class=".btn">#2684</a>
            </td>
            <td>
                <b>
                    Add did web method type as a default option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue #2667.

Inspired by the [did methods documentation](https://github.com/hyperledger/aries-cloudagent-python/blob/main/DIDMethods.md). 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 23:37:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2683" class=".btn">#2683</a>
            </td>
            <td>
                <b>
                    Return 404 when schema not found
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Return a 404 from schema get by id endpoints when the schema is not found.

This could probably be applied to other endpoints as well but I'll be going over the anoncreds endpoints in more detail and can look at them when i'm doing that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 20:13:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2679" class=".btn">#2679</a>
            </td>
            <td>
                <b>
                    Fix: Change To Use Timezone Aware UTC datetime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix issue #2678

Based on 0.11.0rc2 code because when I attempt to use the main branch as the base I am getting an error:

```
  File "/app/aries_cloudagent/anoncreds/__init__.py", line 3, in <module>
    from ..config.injection_context import InjectionContext
ImportError: attempted relative import beyond top-level package
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-17 01:16:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2676" class=".btn">#2676</a>
            </td>
            <td>
                <b>
                    Cache TAA by wallet name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The TAA acceptance was being cached at pool level. This caused problems in traction if the tenant changed pods and also TAA acceptance between different tenants in multi-tenant mode.

My understanding is limited in this area. 
I thought maybe I could cache at a wallet level, but I couldn't find a way to do this currently or any other examples in the code base. So, I inject the cache at profile level and then have a different cache key per wallet/tenant.

This will use more cache memory per tenant. Could possibly store the cache for less time.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 22:38:17 +0000 UTC
    </div>
</div>

