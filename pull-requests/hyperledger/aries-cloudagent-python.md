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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1941" class=".btn">#1941</a>
            </td>
            <td>
                <b>
                    Add startup flag --light-weight-webhook to trim down outbound webhook payload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When we create a credential offer with image, the image is repeated in following objects (dict) 
"credential_request", "cred_request", "credential_proposal", "cred_proposal", "credential_offer", "cred_offer", "credential_preview", "cred_preview", "values", "credentials~attach", "offers~attach"

a Credential offer with 30KB image resulted in a webhook sized at 227KB in my use case and resulted HTTP 413 as well as unnecessary stress on WAF rule regex processes on those encrypted string and base64 image string.

This startup flag will remove those objects only on outbound webhook and size went down to 7KB at most.
I did preserve 1 object "cred_issue" which has the "rev_reg_id" and "cred_rev_id".

To me this is a more like a nice to have flag if someone ever encounter problem with image and webhook.

Previous related discussion
[PR #725](https://github.com/hyperledger/aries-cloudagent-python/pull/725)
[Issue #1222](https://github.com/hyperledger/aries-cloudagent-python/issues/1222)

Signed-off-by: Victor Lee <victorlee0505@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 20:48:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1940" class=".btn">#1940</a>
            </td>
            <td>
                <b>
                    Fix: OOB - Handling of minor versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill [gill.shaanjots@gmail.com](mailto:gill.shaanjots@gmail.com)

- resolve #1917
- Fixes the following error:
```
File "/home/indy/.venv/lib/python3.6/site-packages/aries_cloudagent/utils/classloader.py", line 97, in load_class
   |     if "." in class_name:
   | TypeError: argument of type 'NoneType' is not iterable
```
- Working on adding minor changes for adding OOB 1.1 and a mechanism for ACA-Py to respond with the same supported version, basically, `handshake-reuse-accepted 1.1` for `handshake-reuse 1.1` and `handshake-reuse-accepted 1.0` for `handshake-reuse 1.0`. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 20:22:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1938" class=".btn">#1938</a>
            </td>
            <td>
                <b>
                    Endorser write DID transaction
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
        Created At 2022-09-12 06:10:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1937" class=".btn">#1937</a>
            </td>
            <td>
                <b>
                    Redis Plugins [redis_cache & redis_queue] related updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>

- The `RedisPlugins.md` documentation depends on the approval of [aries-acapy-cache-redis PR](https://github.com/Indicio-tech/aries-acapy-cache-redis/pull/9). Will take it out of draft once that PR is approved.
- `run_docker` file has been updated to accept `NETWORK_NAME` env variable. This is needed when loading up an ACA-Py agent with either `redis_queue` or `redis_cache` plugin when connected to a redis cluster, as the cluster requires a docker network with a predefined subnet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 02:58:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1935" class=".btn">#1935</a>
            </td>
            <td>
                <b>
                    Delete sonarcloud.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Disable automatic sonarcloud

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 15:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1934" class=".btn">#1934</a>
            </td>
            <td>
                <b>
                    Fix/endpoint attrib structure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the solution discussed in #1928 to resolve an issue with the endpoint attrib structure. We have brought the structure into alignment with the did:sov specification by removing the nested endpoint structure and ensuring that service types `profile` and `linked_domains` can be used. This solution is interoperable with AFJ, which also supports endpoint attrib data in the following manner:

```json
{
  "endpoint": "https://example.com",
  "types": ["did-communication", ...],
  "routingKeys": [...],
  "profile": "https://example.com/profile",
  "linked_domains": "https://example.com/linked-domains",
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 23:32:04 +0000 UTC
    </div>
</div>

