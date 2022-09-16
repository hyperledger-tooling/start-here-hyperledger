---
layout: default
title: hlf-connector
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hlf-connector
---

# hlf-connector <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-connector){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    update springboot version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. update spring version to 2.7.1
2. update jdk version to 11
3. update conflicted dependencies 
4. fix null pointer issue when EventPublishService bean is not instantiated

Signed-off-by: weihong-ou <weihong.ou@walmart.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 17:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Increment version after release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">auto-version-increment</span>
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 15:57:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Fixes for event listening
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                EventListener annotation is redundant in the code which is causing error with events.enable as true while the application is bootstrapping

Signed-off-by: n0s09by <Nidhi.singh0@walmart.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 15:07:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Increment version after release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">auto-version-increment</span>
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 18:31:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Add init_required request param for '/approved-organisations' API
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
        Created At 2022-09-14 17:55:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Increment version after release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">auto-version-increment</span>
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 16:52:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Increment version after release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">auto-version-increment</span>
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 16:22:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Populate init flag from incoming request for fetching approved Orgs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains the changeset for populating the `init` property of lifecycleCheckCommitReadinessRequest from the incoming `ChaincodeOperationsModel` passed by the client rather than setting it default as true.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 13:23:26 +0000 UTC
    </div>
</div>

