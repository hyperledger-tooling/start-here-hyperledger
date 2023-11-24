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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2623" class=".btn">#2623</a>
            </td>
            <td>
                <b>
                    0.10.5
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
        Created At 2023-11-21 22:54:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2622" class=".btn">#2622</a>
            </td>
            <td>
                <b>
                    fix(backport): report presentation result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a backport of #2615 for the 0.10.x branch of releases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 21:23:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2618" class=".btn">#2618</a>
            </td>
            <td>
                <b>
                    fix: wallet type help text out of date
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2617 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 05:28:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2615" class=".btn">#2615</a>
            </td>
            <td>
                <b>
                    fix: report presentation result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR ensures that the result of verifying the presentation for JSON-LD Credentials is factored into the final `verified` status.

cc @andrewwhitehead  @swcurran 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 18:20:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2614" class=".btn">#2614</a>
            </td>
            <td>
                <b>
                    fix: typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: typos
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-19 12:21:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2613" class=".btn">#2613</a>
            </td>
            <td>
                <b>
                    0.11.0rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note the new "dashless" rc version number.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 20:01:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2612" class=".btn">#2612</a>
            </td>
            <td>
                <b>
                    :bug: fix wallet_update when only `extra_settings` requested
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor bug fix: `wallet_update` has a condition:

```py
    if all(
        v is None for v in (wallet_webhook_urls, wallet_dispatch_type, label, image_url)
    ):
        raise web.HTTPBadRequest(reason="At least one parameter is required.")
```

This ignores the newly added `extra_settings`, and so trying to update a wallet with only `extra_settings` in the request raises a faulty Bad Request: "At least one parameter is required."

This PR simply adds `extra_settings` to the list of possible parameters.

Edit: I moved the default value of `extra_settings` to be set in the `get_extra_settings_dict_per_tenant` call. If `extra_settings` defaults to `{}` immediately, then the `v is None` check for `extra_settings` is never True.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 10:13:37 +0000 UTC
    </div>
</div>

