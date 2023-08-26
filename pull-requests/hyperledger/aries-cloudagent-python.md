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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2448" class=".btn">#2448</a>
            </td>
            <td>
                <b>
                    0.10.0-rc2
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
        Created At 2023-08-25 21:55:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2447" class=".btn">#2447</a>
            </td>
            <td>
                <b>
                    fix: ignore duplicate record errors on add key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a bandaid solution to prevent routing keys from being stored for multiple DIDs. It would be nice to correct behavior of the DIDDoc class to not turn routing keys into values in the publicKey list and then claiming that the DID is the controller (with no evidence). However, given the impending replacement of this behavior with did:peer, it doesn't seem worth it to go through that effort right now.

cc @swcurran @WadeBarnes and others
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 18:20:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2446" class=".btn">#2446</a>
            </td>
            <td>
                <b>
                    fix: more doc corrections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2445. ACA-Py's `DIDDoc` class performs transformations prior to storing. This PR accounts for these transformations better.

cc @WadeBarnes @nodlesh
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 21:14:07 +0000 UTC
    </div>
</div>

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

