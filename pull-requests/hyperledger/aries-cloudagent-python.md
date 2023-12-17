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
                The TAA acceptance was being cached at pool level. This caused problems if the connection changed pools and also TAA acceptance between different tenants in multi-tenant mode.

My understanding is limited in this area. My first instinct was to use a cache that was at a tenant/wallet specific level. I couldn't find a way to do this currently or any other examples in the code base. So, instead I inject the cache at profile level and then have a different cache key per wallet/tenant.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 22:38:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2674" class=".btn">#2674</a>
            </td>
            <td>
                <b>
                    docs: create design doc for adding W3C VC format support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains one main document:

- `AnoncredsW3CCompatibility.md` - the design document for implementing w3c vc/vp format support
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 20:52:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2672" class=".btn">#2672</a>
            </td>
            <td>
                <b>
                    Anoncreds - Add unit testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds unit tests for routes, holder, verifier, issuer.

![Screenshot from 2023-12-13 10-50-52](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/96589ed6-0add-4cef-bc64-66974229eacd)

There is still more unit testing to do. Mainly the `revocation.py` file. Also, there was a tricky part with scanning the wallet in holder and using `async for` I haven't figured out yet. Also there is some error handling I haven't covered. 

I tried to create objects with the `anoncreds` library as much as possible to catch problems in the future when using the library. When I couldn't manage to make that work I would mock the object a minimally as possible. I also had some trouble creating some DB/wallet `Entry` responses. To get around this i created some minimal class objects. These are used in holder and issuer files.

I made 2 small changes to src code. In verifier.py changed an error handling message and in holder.py added the mime-types attribute constant that seemed to be missing.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 19:10:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2670" class=".btn">#2670</a>
            </td>
            <td>
                <b>
                    Remove if condition which checks if the `credential.type` array is equal to 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses  #2669

There is currently a validation that prevents credential with only the base type from being signed. The data model spec states that additional credential types are optional. This also prevents conforming to some test-suites where [single credential type](https://github.com/w3c/vc-data-model-2.0-test-suite/blob/main/tests/input/credential-ok.json) credentials are used as test data.

This is a minor change with no impact.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 04:47:04 +0000 UTC
    </div>
</div>

