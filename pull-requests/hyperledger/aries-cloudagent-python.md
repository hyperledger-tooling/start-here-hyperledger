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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1645" class=".btn">#1645</a>
            </td>
            <td>
                <b>
                    Fix DIFPresFormatHandler returning invalid V20PresExRecord on presentation verification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We noticed that a `V20PresExRecord` which is returned by the present-proof v2.0 `/verify-presentation` endpoint does not match its schema when DIF format is used to request a presentation. Because of this, parsing it into a Kotlin class fails:
`com.squareup.moshi.JsonDataException: Expected one of [true, false] but was True at path $.verified`

Fixed this by applying json.dumps() when setting `pres_ex_record.verified` - just like it's done in the indy handler.

However, couldn't `verified` be a boolean instead of a string? I found comments in the schema and in the indy handler saying it has to be a string to be used as a tag (that was my takeaway at least ;) ), but I couldn't find where it is actually declared or used that way.

Signed-off-by: Roman Reinert <roman.reinert@gematik.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 16:50:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1643" class=".btn">#1643</a>
            </td>
            <td>
                <b>
                    feat: accept taa using config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds option to accept the TAA using config parameters in addition to the Admin API and using TTY.

The TAA can be accepted by providing a valid acceptance mechanism, and specifying the version. This is to make sure newer versions of the TAA aren't automatically accepted. If the version does not match, or the acceptance mechanism doesn't exist in the aml, an error is thrown and the process is terminated (this seems fine to me as it is run on startup and can be fatal to using the agent).

The configuration is as follows:

```
--accept-taa on_file 1.0
```

or in the yml config:

```yml
accept-taa: [on_file, 1.0]
```

Fixes #1532 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 12:47:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1642" class=".btn">#1642</a>
            </td>
            <td>
                <b>
                    Pin markupsafe at version 2.0.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Temporary fix due to breaking changes in the dependency.

The 2.2 branch of aiohttp-apispec requires Jinja2 < 3, while its 3.0 (beta) branch supports newer Jinja2 versions which would likely also bypass this issue. We can either test out the current beta or wait for a new release there.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 00:50:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1638" class=".btn">#1638</a>
            </td>
            <td>
                <b>
                    Fix auto connection response not being properly mediated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Connection responses associated with an invite that was created with mediation were not properly reporting the mediators endpoint and keys when automatically sent after receiving a connection request. This PR fixes this issue and also does some minor code clean up.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 18:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1637" class=".btn">#1637</a>
            </td>
            <td>
                <b>
                    feat: query connections by their_public_did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now that `their_public_did` is saved as a tag (https://github.com/hyperledger/aries-cloudagent-python/pull/1543), we can use it to filter connections made with a specific public did.

This PR adds the filter option to the get all connections endpoint. Same as with #1453, this will only work for connections made after PR #1453 was merged or if the upgrade command has been run
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 10:01:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1633" class=".btn">#1633</a>
            </td>
            <td>
                <b>
                    Move database operations inside the session context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## What is this PR for?
- Error state saving was done when the session could be already disposed

Signed-off-by: Andraž Cuderman <andraz.cuderman@global.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 13:07:37 +0000 UTC
    </div>
</div>

