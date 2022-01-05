---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1778" class=".btn">#1778</a>
            </td>
            <td>
                <b>
                    Docs/Build fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

There was a small error in build documentation reported in the chat. This PR fixes it

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

None

### Benefits

<!-- What benefits will be realized by the code change? -->

Fixed docs

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 19:40:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1776" class=".btn">#1776</a>
            </td>
            <td>
                <b>
                    Added possibility to configure max past time of transaction created_time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">help wanted</span><span class="chip">question</span><span class="chip">1.x</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
This is PoC of adding possibility of configuration:
https://iroha.readthedocs.io/en/develop/develop/api/queries.html?highlight=24%20hours#validation
to be different than 24 hours before current time.

**It is just PoC, so it needs to be consult with somebody.**

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Possibility of additional param configuration
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Default behavious is without changes, so I assume none drawbacks
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*
After changing the value in config the changes were tested with the code (20 hours vs 40 hours before current time):
```
import datetime
import os
import binascii
from iroha import IrohaCrypto, Iroha, IrohaGrpc, primitive_pb2
from functools import wraps


IROHA_HOST_ADDR = os.getenv('IROHA_HOST_ADDR', 'localhost')
IROHA_PORT = os.getenv('IROHA_PORT', '50051')

net = IrohaGrpc(f'{IROHA_HOST_ADDR}:{IROHA_PORT}')

ADMIN_ACCOUNT_ID = os.getenv('ADMIN_ACCOUNT_ID', 'admin@test')
ADMIN_PRIVATE_KEY = os.getenv(
    'ADMIN_PRIVATE_KEY', 'f101537e319568c765b2cc89698325604991dca57b9716b58016b253506cab70')
iroha_admin = Iroha(ADMIN_ACCOUNT_ID)


DOMAIN = 'test'

private_key = '1234567890123456789012345678901234567890123456789012345678901234'
public_key = IrohaCrypto.derive_public_key(private_key)


def trace(func):
    """ A decorator for tracing methods' begin/end execution points """

    @wraps(func)
    def tracer(*args, **kwargs):
        name = func.__name__
        print(f'\tEntering "{name}"')
        result = func(*args, **kwargs)
        print(f'\tLeaving "{name}"\n')
        return result

    return tracer

@trace
def create_account(user_account_short_id: str, user_public_key: str, created_time: datetime):
    created_time_ts = get_timestamp_milliseconds(created_time)
    tx = iroha_admin.transaction([
        iroha_admin.command('CreateAccount', account_name=user_account_short_id, domain_id=DOMAIN,
                            public_key=user_public_key)
    ], created_time=created_time_ts)
    IrohaCrypto.sign_transaction(tx, ADMIN_PRIVATE_KEY)
    send_transaction_and_print_status(tx)


def send_transaction_and_print_status(transaction):
    hex_hash = binascii.hexlify(IrohaCrypto.hash(transaction))
    print(f'Transaction "{get_command_from_tx(transaction)}" hash = {hex_hash}, '
          f'creator = {transaction.payload.reduced_payload.creator_account_id}')
    net.send_tx(transaction)
    for status in net.tx_status_stream(transaction):
        print('\t\t', status)
    result = status[0]
    if result != 'COMMITTED':
        raise Exception(f'Command {get_command_from_tx(transaction)} failed! {status}')


def get_command_from_tx(tx):
    commands_from_tx = []
    for command in tx.payload.reduced_payload.__getattribute__("commands"):
        listed_fields = command.ListFields()
        commands_from_tx.append(listed_fields[0][0].name)
    return commands_from_tx[0]

@trace
def get_account_transactions(iroha_connection, account_id: str, account_key: str):
    query = iroha_connection.query('GetAccountTransactions', account_id=account_id, page_size=10)

    IrohaCrypto.sign_query(query, account_key)

    response = net.send_query(query)
    print(f'\n----- Transactions of account {account_id}:\n', response)


def get_timestamp_milliseconds(dt: datetime.datetime):
    ts = dt.timestamp()
    return round(ts*1000)


if __name__ == '__main__':
    current_time = datetime.datetime.now()
    old_time = current_time - datetime.timedelta(hours=23)
    even_older_time = current_time - datetime.timedelta(hours=40)

    print(current_time, "miliseconds:", get_timestamp_milliseconds(current_time))
    print(old_time, "miliseconds:", get_timestamp_milliseconds(old_time))
    print(even_older_time, "miliseconds:", get_timestamp_milliseconds(even_older_time))

    create_account(user_account_short_id='a1', user_public_key=public_key, created_time=current_time)
    create_account(user_account_short_id='a2', user_public_key=public_key, created_time=old_time)
    create_account(user_account_short_id='a3', user_public_key=public_key, created_time=even_older_time)

    get_account_transactions(iroha_admin, ADMIN_ACCOUNT_ID, ADMIN_PRIVATE_KEY)
```
<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 18:10:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1775" class=".btn">#1775</a>
            </td>
            <td>
                <b>
                    [fix] #1714: Compare PeerId only by key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Egor Ivkov <e.o.ivkov@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Compare PeerId only by key.
Comparison is done by public key only, so that full domain names can be present in trusted peers and local address in this peer config without a conflict.

The problem was found during longevity stand setup. When:
1. `TORII_P2P_ADDR` was `0.0.0.0:1337`
2. `SUMERAGI_TRUSTED_PEERS` had `[{"address": "some.test.domain:1337", ...}, ... ]`

The peers therefore did not discover themselves in trusted peers and were not considering themselves to be validators, leading to genesis block not being committed.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 14:35:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1773" class=".btn">#1773</a>
            </td>
            <td>
                <b>
                    [fix] #1772: Fix after #1764
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
Apply additional review comments of #1764

### Issue
Close #1772

### Benefits

### Possible Drawbacks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 13:07:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1770" class=".btn">#1770</a>
            </td>
            <td>
                <b>
                    Merge develop into main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Adds features and fixes for Iroha v1.4-rc.1 in ```main```.
- feature/healthcheck
- feature/rocksdb_metrics
- feature/syncing_node

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 09:46:24 +0000 UTC
    </div>
</div>

