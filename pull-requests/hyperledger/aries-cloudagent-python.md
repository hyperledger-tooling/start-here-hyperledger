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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2605" class=".btn">#2605</a>
            </td>
            <td>
                <b>
                    Default connection_id to None to account for Connectionless Proofs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a small change in response to [this issue and conversation](https://github.com/hyperledger/aries-cloudagent-python/issues/2597).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 21:50:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2604" class=".btn">#2604</a>
            </td>
            <td>
                <b>
                    chore: correct type hints on base record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a small tweak to correct the type hints on base record and related base classes. These are base classes used widely both within ACA-Py and in plugins. Having these types corrected will solve a cascade of static type checking errors.

These aren't strictly necessary errors to fix but they sure make my life as a developer easier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 20:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2603" class=".btn">#2603</a>
            </td>
            <td>
                <b>
                    black formatter extension configuration update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See PR #2602

The black formatter extension was updated last night and the current configuration doesn't work. This simple change corrects the loading error.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 20:04:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2602" class=".btn">#2602</a>
            </td>
            <td>
                <b>
                    Update Devcontainer pytest ruff black
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bring in changes from commit 48e24043f0a5ad89b5e6e808c26b9552a8856abd.

Updates devcontainer to run pytests in Testing view and integrate `ruff` and `black` into the IDE better.

One change is in devcontainer.json, setting the black formatter to "useBundled"...  They updated their extension last night. The change is also needed in the main branch.

```
Published 2022-04-14, 14:24:13
Last released 2023-11-08, 02:11:58
Last updated 2023-11-08, 10:56:39
Identifier ms-python.black-formatter
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 19:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2600" class=".btn">#2600</a>
            </td>
            <td>
                <b>
                    Add ConnectionProblemReport handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Leaving this here as a starting point or example.

See issues #2530 and #2599.

I think we would want to address #2599 first (or include in here) and get the error classes fixed up, then the handler will actually be effective.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 16:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2596" class=".btn">#2596</a>
            </td>
            <td>
                <b>
                    WIP initial code migration from anoncreds-rs branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 21:07:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2595" class=".btn">#2595</a>
            </td>
            <td>
                <b>
                    Issue 2570 devcontainer ruff, black and pytest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2570 

Adding `--ruff` to the `pytest` configuration in `pyproject.toml` adversely affects the `devcontainer`: the Testing view does not load properly (tests are discovered but not listed). It is convenient to have those tests loaded in the Testing view for debugging and troubleshooting, allowing the developer to isolate and repeatedly run individual files/tests quickly.

One important caveat is the devcontainer creates its own `.pytest.ini` file (it is gitgnored) which overrides the configuration in [pyproject.toml](./pyproject.toml). `ruff` will ignore this file and continue to use the pyproject configuration. The `ruff` extension is also explicitly configured to use the pyproject configuration. Creating a `.pytest.ini` file when the container is built means that file will continue to exist on the file system outside of the container. So if a developer flips between using the devcontainer and running commands directly on their system they will pick up the `.pytest.ini` file which would not run `ruff` check when calling `python -m pytest .` on the local machine. These changes do *NOT* impact `./scripts/run_tests` or `./scripts/run_tests_indy` - those will continue to use the pyproject configuration.

This PR adds extensions for `ruff` and `black`, setting up `black` as the default formatted and integrating `ruff` into the editor/command palette.

Updates have been made to the [devcontainer](./devcontainer.md) README to inform users/developers of the changes and caveats.

*NOTE* - the `ruff` version has been updated to match the extension.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-06 20:29:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2591" class=".btn">#2591</a>
            </td>
            <td>
                <b>
                    Goal and Goal Code in invitation URL.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a unit test to ensure goal/goal code are in the encoded invitation URL.

Fixes #2583 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 23:23:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2590" class=".btn">#2590</a>
            </td>
            <td>
                <b>
                    Fix Issue #2589 TypeError When There Are No Nested Requirements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added `if` statement, same as in calling function `create_vp`, to the called function `apply_requirements`. Since the former calls `apply_requirements` in both cases (`if req.nested_req` or not), the called function should handle both cases as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 18:49:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2588" class=".btn">#2588</a>
            </td>
            <td>
                <b>
                    Anoncreds rs - draft PR to monitor differences between the branch and main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 16:25:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2587" class=".btn">#2587</a>
            </td>
            <td>
                <b>
                    feat: use a local static cache for commonly used contexts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [Related to this issue](https://github.com/hyperledger/aries-cloudagent-python/issues/2581)

* Package a list of commonly used contexts 
* Replace the context loader from pyld with `StaticCacheJsonLdDownloader`
* `StaticCacheJsonLdDownloader` resolves contexts from local package in priority, then delegates to a downloader
* As of now, `JsonLdDocumentDownloader` and `JsonLdDocumentParser` are simply lifted from pyld in a way that decouples downloading and parsing JSON-LD documents.
* Tests are mostly drafts, waiting for feedback before investing time there.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 12:57:49 +0000 UTC
    </div>
</div>

