---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/724" class=".btn">#724</a>
            </td>
            <td>
                <b>
                    fix-646: Implemented Re-try failed scenarios
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for the [issue ](https://github.com/hyperledger/aries-agent-test-harness/issues/646)

Changes made
1) Added a before_feature hook to implement retry failed scenarios.
2) Passing the overriding variable TEST_RETRY_ATTEMPTS_OVERRIDE via manage.py to docker environment

Note : Found $DOCKER_ENV is not passed to the docker run command on runTests() function. So adding that too.

How to run:
There are two ways to overide the no of attempts for re-try failed scenarios

1) Add the variable **test_retry_attempts** in the **behave.ini** like below

> test_retry_attempts = 2

2) Pass the variable **TEST_RETRY_ATTEMPTS_OVERRIDE** as environment variable while running test or through deployment yaml files.

> eg: TEST_RETRY_ATTEMPTS_OVERRIDE=2 ./manage run -d acapy -b javascript -t @AcceptanceTest

Screenshots

![image](https://github.com/hyperledger/aries-agent-test-harness/assets/79985154/6742443e-4260-46cc-8017-46ec3264dc6c)
![image](https://github.com/hyperledger/aries-agent-test-harness/assets/79985154/650ce2cd-d041-4c82-bb3a-5246d06a1b3d)
![image](https://github.com/hyperledger/aries-agent-test-harness/assets/79985154/c0abf141-7400-4b3e-b9cd-eeab3061fa65)
![image](https://github.com/hyperledger/aries-agent-test-harness/assets/79985154/c35a3f08-400b-4a83-9fbf-3dbf99c2f770)



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 20:07:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/723" class=".btn">#723</a>
            </td>
            <td>
                <b>
                    aries-vcx: implement did-exchange protocol (with peer did support)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 08:46:21 +0000 UTC
    </div>
</div>

