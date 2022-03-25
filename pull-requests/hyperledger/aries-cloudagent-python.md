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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1690" class=".btn">#1690</a>
            </td>
            <td>
                <b>
                    Fix: DIF proof proposal when creating bound presentation request [Issue#1687]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
- resolve #1687 
- So the validation for `/present-proof-v2.0/send-proposal` is working but the problem was that with `auto_respond_presentation_proposal` flag on it would create an invalid bound request from the proposal [`input_descriptors` was not enclosed in `presentation_definition`]. I am surprised that I didn't catch this earlier.
- @swcurran According to the [RFC](https://github.com/hyperledger/aries-rfcs/blob/main/features/0510-dif-pres-exch-attach/README.md#examples-propose-presentation), the `propose-presentation` message only expects `input_descriptors` and no `options` [for `challenge` and/or `domain`]. With auto flag, there will be no opportunity to add a domain to the request, so I have updated the schema to allow `options` in the `propose-presentation` message. `challenge` is always required for verifying presentation, if `options` is not specified then it is randomly assigned.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 08:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1688" class=".btn">#1688</a>
            </td>
            <td>
                <b>
                    Remove references to play with von
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 17:05:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1676" class=".btn">#1676</a>
            </td>
            <td>
                <b>
                    Fix DIF PresExch and OOB request_attach delete unused connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                - resolve #1608 
- resolve #1609
- Fixed an issue with OOB workflow, unused connections were not deleted with invitation containing request attachments.
- DIF PE: fixed an issue where numerical comparisons are requested for an attribute that could be included as a number string.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 16:00:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1675" class=".btn">#1675</a>
            </td>
            <td>
                <b>
                    [#1674] Add basic DOCKER_ENV logging for run_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 15:32:03 +0000 UTC
    </div>
</div>

