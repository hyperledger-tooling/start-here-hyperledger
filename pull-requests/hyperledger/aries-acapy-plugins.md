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
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/461" class=".btn">#461</a>
            </td>
            <td>
                <b>
                    Release for aries-cloudagent v0.12.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Release v0.12.1
##### The latest supported versions of aries-cloudagent for each plugin are as follows:

| Plugin Name | Supported aries-cloudagent version |
| --- | --- |
|basicmessage_storage | 0.12.1|
|connection_update | 0.12.1|
|firebase_push_notifications | 0.12.1|
|kafka_events | 0.12.1|
|multitenant_provider | 0.12.1|
|oid4vci | 0.12.1|
|redis_events | 0.12.1|
|rpc | 0.12.1|
***
 -  #### Plugins upgraded this release: 
	 -  basicmessage_storage 
	 -  connection_update 
	 -  firebase_push_notifications 
	 -  kafka_events 
	 -  multitenant_provider 
	 -  oid4vci 
	 -  redis_events 
	 -  rpc
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 15:49:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/460" class=".btn">#460</a>
            </td>
            <td>
                <b>
                    OID4VCI plugin - Fix delete  exchange-supported records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quick fix on ./oid4vci/exchange-supported/records delete. There is a typo that duplicates the "credential supported identifier" as a parameter causing deletes to fail.

FYI @dbluhm 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-15 15:25:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/459" class=".btn">#459</a>
            </td>
            <td>
                <b>
                    update release PR workflow token
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I tried using the new PAT token for the PR workflow but it didn't work. I'm thinking it possibly has the permissions required to make the release but not the PR. The normal GITHUB_TOKEN should have the permissions to make the PR so i'm trying that.

![Screenshot from 2024-05-14 08-29-27](https://github.com/hyperledger/aries-acapy-plugins/assets/31809382/4605bbb9-cb29-4a9e-81b8-a55edae41262)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 15:32:08 +0000 UTC
    </div>
</div>

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

