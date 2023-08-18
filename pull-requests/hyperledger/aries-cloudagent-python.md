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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2429" class=".btn">#2429</a>
            </td>
            <td>
                <b>
                    Don't run Snyk on forks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2428
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 18:35:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2427" class=".btn">#2427</a>
            </td>
            <td>
                <b>
                    Update /schemas to use anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP needs feedback to determine if this is the right direction.

Have updated:
- [All /schemas routes](https://github.com/hyperledger/aries-cloudagent-python/blob/2565fe84e2716fcda44a3b1bb32095e9c6fd62bd/aries_cloudagent/messaging/schemas/routes.py)
- [POST /credential-definitions](https://github.com/hyperledger/aries-cloudagent-python/blob/2565fe84e2716fcda44a3b1bb32095e9c6fd62bd/aries_cloudagent/messaging/credential_definitions/routes.py#L167)
- [GET /credential-definitions/<id>](https://github.com/hyperledger/aries-cloudagent-python/blob/2565fe84e2716fcda44a3b1bb32095e9c6fd62bd/aries_cloudagent/messaging/credential_definitions/routes.py#L483)
- [POST /revocations/revoke](https://github.com/hyperledger/aries-cloudagent-python/blob/1f6cbf6635fc53e5c945b95353bff48706ed9638/aries_cloudagent/revocation/routes.py#L440)

Enabled all "broken" BDD tests (except in sign-transaction due to endorser).

More credential definition routes to fix as well as revocation. The BDD tests pass now, so that means BDD does not do complete coverage.

Will have to address the pytests at some point too.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 02:14:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2425" class=".btn">#2425</a>
            </td>
            <td>
                <b>
                    Per Tenant Logging - Complete Implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #2359 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 17:56:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2423" class=".btn">#2423</a>
            </td>
            <td>
                <b>
                    the anoncreds proof presentation with schema restriction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                missed this file... 🤦 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 22:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2421" class=".btn">#2421</a>
            </td>
            <td>
                <b>
                    Issue #2250 Nightly publish workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This issue resolves #2250

Here I have created a GitHub workflow that will execute the tests just as they are handled in `nightly-tests.yml` excluding the indy tests as mentioned in this comment.

https://github.com/hyperledger/aries-cloudagent-python/issues/2250#issuecomment-1674918887

The workflow acts as follows
```python
run nightly tests
If (tests are successful):
   build a nightly release
   publish this release with the `nightly` tag
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 15:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2420" class=".btn">#2420</a>
            </td>
            <td>
                <b>
                    Issue #2419 InvalidClientTaaAcceptanceError time too precise error if container timezone is not UTC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds timezone.utc to datetime.combine to ensure time will be midnight in UTC regardless of the default timezone
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 23:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2418" class=".btn">#2418</a>
            </td>
            <td>
                <b>
                    Enable Snyk scanning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                addresses #2087 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 20:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2416" class=".btn">#2416</a>
            </td>
            <td>
                <b>
                    feat: Proof Negotiation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a rebased version of #2033. Thank you for your contributions, @Przytua!

I think these changes are likely to be better suited to a new endpoint (i.e. `POST /present-proof/{pres_ex_id}/counter-request` or something) rather than changing the behavior of `POST /present-proof/{pres_ex_id}/request`. I'll open this as a draft for now and look at making these changes when I can.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 19:01:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2415" class=".btn">#2415</a>
            </td>
            <td>
                <b>
                    Remove Indy tests from workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed recently and captured in #2402, this PR removes Indy specific tests from PR test runs. This also adjusts other images and examples in the demo folder to use the non-indy variant of images.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 14:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2414" class=".btn">#2414</a>
            </td>
            <td>
                <b>
                    0.10.0-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 18:38:25 +0000 UTC
    </div>
</div>

