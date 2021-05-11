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
                PR <a href="https://github.com/hyperledger/iroha/pull/1008" class=".btn">#1008</a>
            </td>
            <td>
                <b>
                    Add simple actor framework
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: i1i1 <vanyarybin1@live.ru>

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

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 15:29:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1007" class=".btn">#1007</a>
            </td>
            <td>
                <b>
                    Add nice panic and error reporters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                https://jira.hyperledger.org/browse/IR-1019
Signed-off-by: i1i1 <vanyarybin1@live.ru>

### Description of the Change

Add panic handler with stacktrace and error reporting. Add error reporter for `iroha_error::Error`. Now it can be nicely formatted  everywhere if needed.

### Benefits

More context where needed on errors.

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-08 13:16:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1006" class=".btn">#1006</a>
            </td>
            <td>
                <b>
                    Docs: Documentation about metric flags
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

Adds description of metrics flags to the documentation

### Benefits

S'more docs

### Possible Drawbacks 

Might need to change the phrasing in the --help too but that is not a critical thing. 

Resolves #845 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 22:06:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1004" class=".btn">#1004</a>
            </td>
            <td>
                <b>
                    Refactor/remove rxcpp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - SE field in Irohad class
- Remove rxcpp from TransactionProcessorImpl
- Use any_range in BlockLoader interface
- Remove rxcpp from Synchronizer
- Remove rxcpp from Simulator
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 12:48:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    826 fix grpc msg size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # The problem iroha freezes inside GRPC
when waiting response to a big (more than 4MB) message.

# Steps to reproduce
Send long transactions batch (more than 250)

```
from iroha import *


def public_key_from_private(private_key: str):
    return IrohaCrypto.derive_public_key(private_key).decode('utf-8')


def send_signed_batch_transaction(txs, net):
    net.send_txs(txs)
    for tx in txs:
        print(f'Transaction hash = {calculate_hash_of_transaction(tx)}')
        for status_name, status_code, error_code in net.tx_status_stream(tx, timeout=20):
            print(f'\tstatus_name:{status_name}, status_code:{status_code}, error_code:{error_code}')


def calculate_hash_of_transaction(transaction_with_payload):
    h = IrohaCrypto.hash(transaction_with_payload)
    return binascii.hexlify(h).decode("utf-8")


if __name__ == '__main__':
    IROHA_HOST_ADDR = os.getenv('IROHA_HOST_ADDR', 'localhost')
    IROHA_PORT = os.getenv('IROHA_PORT', '50051')
    ADMIN_ACCOUNT_ID = os.getenv('ADMIN_ACCOUNT_ID', 'admin@test')
    ADMIN_PRIVATE_KEY = os.getenv('ADMIN_PRIVATE_KEY', 'f101537e319568c765b2cc89698325604991dca57b9716b58016b253506cab70')

    iroha = Iroha(ADMIN_ACCOUNT_ID)
    net = IrohaGrpc(f'{IROHA_HOST_ADDR}:{IROHA_PORT}',max_message_length=400*1024*1024)

    new_user_private_key = '1234567890123456789012345678901234567890123456789012345678901234'
    new_user_public_key = public_key_from_private(new_user_private_key)

    accounts_to_create = 250

    txs = []
    for i in range(accounts_to_create):
        txs.append(
            iroha.transaction([
                iroha.command('CreateAccount', account_name=f'1p_account_{i}', domain_id='test', public_key=new_user_public_key)
            ]))

    iroha.batch(txs, atomic=False)

    for tx in txs:
        IrohaCrypto.sign_transaction(tx, ADMIN_PRIVATE_KEY)

    send_signed_batch_transaction(txs, net)

```
After this iroha freezes and python script results with 
```
        status = StatusCode.DEADLINE_EXCEEDED
        details = "Deadline Exceeded"
        debug_error_string = "{"created":"@1619454477.951686000","description":"Error received from peer ipv6:[::1]:50051","file":"src/core/lib/surface/call.cc","file_line":1068,"grpc_message":"Deadline Exceeded","grpc_status":4}"
```



# Result after fix

> Received message larger than max (4207140 vs. 4194304)

```
> python3 batch_test.py
Traceback (most recent call last):
  File "/batch_test.py", line 47, in <module>
    send_signed_batch_transaction(txs, net)
  File "/batch_test.py", line 9, in send_signed_batch_transaction
    net.send_txs(txs)
  File "/usr/local/lib/python3.9/site-packages/iroha/iroha.py", line 396, in send_txs
    self._command_service_stub.ListTorii(tx_list, timeout=timeout)
  File "/usr/local/lib/python3.9/site-packages/grpc/_channel.py", line 923, in __call__
    return _end_unary_response_blocking(state, call, False, None)
  File "/usr/local/lib/python3.9/site-packages/grpc/_channel.py", line 826, in _end_unary_response_blocking
    raise _InactiveRpcError(state)
grpc._channel._InactiveRpcError: <_InactiveRpcError of RPC that terminated with:
        status = StatusCode.RESOURCE_EXHAUSTED
        details = "Received message larger than max (4207140 vs. 4194304)"
        debug_error_string = "{"created":"@1619454844.395104000","description":"Error received from peer ipv6:[::1]:50051","file":"src/core/lib/surface/call.cc","file_line":1068,"grpc_message":"Received message larger than max (4207140 vs. 4194304)","grpc_status":8}"
>

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 19:27:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1002" class=".btn">#1002</a>
            </td>
            <td>
                <b>
                    PR template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sara <lira.lemur@gmail.com>

### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

Adding PR template instructions on automatically resolving GH issues. Like here:

Resolves #828

### Benefits

Cool automated issue management

### Possible Drawbacks 

If it actually does not solve the issue?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 13:58:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    Feature/main merge
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

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 09:59:41 +0000 UTC
    </div>
</div>

