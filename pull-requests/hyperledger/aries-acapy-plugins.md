---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/450" class=".btn">#450</a>
            </td>
            <td>
                <b>
                    :arrow_up: Bulk upgrade common dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follows up from #449 

Uses find-replace-all to upgrade the following dependencies across pyptoject.toml files:
- aiohttp
- bcrypt
- black
- pydantic
- pytest
- pytest-asyncio
- pytest-cov
- pytest-mock
- pytest-ruff
- rope
- ruff

Also specific to redis-events plugin:
- fastapi
- redis
- uvicorn

Please review commit logs to verify this.

Does not include upgrades to older sub-projects, which are pinned to older python versions:
- kafka_events/kafka_events/v1_0/deliverer/pyproject.toml
- kafka_events/kafka_events/v1_0/http_kafka_relay/pyproject.toml

Note: I added a bash script that helps with applying poetry lock to every relevant directory. May be helpful for future use.

Tada! :tada: This should clear up a bunch of open dependabot PRs, and should hopefully make maintaing this multi-project repo a bit easier

___ 

Side-note: the following:
- oid4vci/integration/afj_runner/pyproject.toml

complains about:
```sh
The dependency name for controller does not match the actual package's name: acapy-controller
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 11:05:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/449" class=".btn">#449</a>
            </td>
            <td>
                <b>
                    :heavy_minus_sign: remove `asynctest` dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaces `asynctest` with `unittest` in all modules

Includes formatting changes from #448. Marking as draft until that one's merged
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 10:03:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    :art: Apply formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We're maintaining a fork of this repo, and to avoid merge conflicts in the future, it'd be helpful if formatting were applied to the codebase.

This just applies `black` formatting and `isort` for import organisation. No other changes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 09:40:06 +0000 UTC
    </div>
</div>

