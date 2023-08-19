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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2436" class=".btn">#2436</a>
            </td>
            <td>
                <b>
                    #2289 Migrate to Poetry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR resolves #2289

I migrated the use of requirements.txt and setup.py over to poetry. The use of multiple requirements.*.txt is replaced with dependency groups in the `pyproject.toml`. I have also added a dedicated `[tool.poetry.group.test.dependencies]` as opposed to the original requirements.dev.txt which contained both developer dependencies and testing dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-19 00:33:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2435" class=".btn">#2435</a>
            </td>
            <td>
                <b>
                    Fix for nightly tests failing on Python 3.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Before the recent support for nightly release tests for Python 3.10 (see the logs [here](https://github.com/hyperledger/aries-cloudagent-python/actions/runs/5861979241/job/15893033620)) were broken this fix corrected the tests by simply replacing  [async_case](https://pypi.org/project/async-case/) with the original [unittest](https://docs.python.org/3/library/unittest.html) library.

A similar issue was resolved for the same incompatibility in #2187

As [async_case](https://pypi.org/project/async-case/) was simply a backport of functionality included since Python 3.8 and acapy supports Python 3.9+ there is no longer a need for [async_case](https://pypi.org/project/async-case/).

Finally, this means we also restore the functionality of 2 additional tests that were previously skipped in #2187

## Including Tests as a Dependency for Nightly Releases
In addition, the current release does not check that the tests for Python 3.10 were successful before building a nightly release. This PR also adds this as a dependency. 


## Additional context
The current source of the error with Python 3.10 is due to [async_case](https://pypi.org/project/async-case/) using 
```python
            loop.run_until_complete(
                asyncio.gather(*to_cancel, loop=loop, return_exceptions=True))
```
as of Python 3.10 the `loop` keyword has been depreciated in [asyncio.gather](https://docs.python.org/3/library/asyncio-task.html#asyncio.gather). 

This leads to the following exception
![image](https://github.com/hyperledger/aries-cloudagent-python/assets/34443260/f25991be-6e62-4a00-a8ab-25e7661f3c40)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 21:13:22 +0000 UTC
    </div>
</div>

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

