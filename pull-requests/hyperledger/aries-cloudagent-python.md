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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1748" class=".btn">#1748</a>
            </td>
            <td>
                <b>
                    Fix: Problem Report webhook - tails file upload failure when creating cred_def
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1743 
- @PaulWen This will dispatch a webhook [topic: `acapy::problem_report`] with the payload containing `cred_def_id` [pthid], `revoc_reg_id` [thid] and the reason. 
I think you expected this information to be presented in either `POST /credential-definitions` or `/topic/revocation_registry` webhook. Within `POST /credential-definitions`, the cred_def is written to the wallet and ledger but the upload of the tails file gets done separately as a registered event [EventBus], so it is difficult to show the error here. With `/topic/revocation_registry` webhook, based upon what I found, it is only triggered for [`init`, `generated`, `posted`, `active`] states.
- Regarding ACA-Py logs, this was already implemented and you should have seen something like:
```
2022-04-27 21:04:45,521 aries_cloudagent.core.event_bus ERROR Error occurred while processing event
Traceback (most recent call last):
  File "/home/indy/aries_cloudagent/core/event_bus.py", line 120, in notify
    await processor()
  File "/home/indy/aries_cloudagent/revocation/routes.py", line 1274, in on_revocation_tails_file_event
    raise RevocationError(err_msg)
aries_cloudagent.revocation.error.RevocationError: Tails file for rev reg W1dd41kbhMNopR5h38PWsm:4:W1dd41kbhMNopR5h38PWsm:3:CL:8:test205:CL_ACCUM:1d809179-3108-4f53-ba1b-a8c57a87d14c failed to upload: Exceeded maximum put attempts
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 22:14:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1747" class=".btn">#1747</a>
            </td>
            <td>
                <b>
                    Updates to Changelog for 0.7.4. RC1 release
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
        Created At 2022-04-27 18:22:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1746" class=".btn">#1746</a>
            </td>
            <td>
                <b>
                    [#1745] Fetch from --genesis-url likely to fail in composed container…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … setup

Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 12:15:58 +0000 UTC
    </div>
</div>

