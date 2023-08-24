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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2443" class=".btn">#2443</a>
            </td>
            <td>
                <b>
                    Add symlink to /home/indy/.indy_client for backwards compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should resolve an issue happening when migrating an indy-based agent to an askar-only image: the home directories will change, however the database will contain references to previously created artifacts (specifically tails files in the case that triggered this fix) that will not be resolvable anymore.

Creating a symlink for `/home/indy/.indy-client/` pointing to `/home/aries/.indy_client` should resolve issues with path resolution without needing to update path references stored in the database.

We could potentially create a symlink between `/home/indy` and `/home/aries`, but I don't like the idea of symlinking home directories.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 00:55:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2442" class=".btn">#2442</a>
            </td>
            <td>
                <b>
                    0.10.0-rc1
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
        Created At 2023-08-24 00:09:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2440" class=".btn">#2440</a>
            </td>
            <td>
                <b>
                    migrate credential definition routes to anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Set existing `/credential-definitions` endpoints to use `anoncreds`.

As per the discussion, the `write_record` methods and endpoints were removed for both schema and cred defs.

Closes #2431 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 22:54:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2439" class=".btn">#2439</a>
            </td>
            <td>
                <b>
                    Draft update to the security policy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A draft PR that builds on the pending new Hyperledger Foundation Security Vulnerability Reporting policy. It too is still a PR -- here: https://github.com/hyperledger/toc/pull/143

This is a proposed instance of the Security.md file for a project.  Once the new Hyperledger policy is merged, and this PR is aligned with that policy, this PR will be ready to be reviewed by the ACA-Py and broader Aries community.

Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 19:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2438" class=".btn">#2438</a>
            </td>
            <td>
                <b>
                    Swap out flake8 in favor of Ruff
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2400.

This PR replaces flake8 with Ruff as suggested by @ff137. I've selected a "reasonable" set of selected and ignored error codes for now. I think we should add/no longer ignore more in the future.

One in particular that I think should have it's own issue raised over is C901 or cyclomatic complexity checks. By default, Ruff sets the threshold at 10. This is a pretty common threshold. There are 81 instances of ACA-Py exceeding that threshold. These are ignored for the time being as it's likely each instance will require individual attention.

I've also moved miscellaneous configuration for dev tools out of `setup.cfg` and translated them into `pyproject.toml`. We'll need to make sure this meshes well with changes in #2436.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 23:03:51 +0000 UTC
    </div>
</div>

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

