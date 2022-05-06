---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/794" class=".btn">#794</a>
            </td>
            <td>
                <b>
                    Do not init apiserver config, until after config reset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                CORS defaults were not being applied any more, after #791 moved the initialization to be alongside all the rest of the HTTP server config.

We were initializing those config prefixes, before we were calling `coreconfig.Reset()`

![image](https://user-images.githubusercontent.com/6660217/167027739-9275f639-fa3e-4d8a-9ea9-a9e722ebabb4.png)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 21:22:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/793" class=".btn">#793</a>
            </td>
            <td>
                <b>
                    Fix links in documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I deleted the previous branch when i noticed my git credentials had not been updated in my signed commits.
This PR still addresses the two links.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 20:17:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/792" class=".btn">#792</a>
            </td>
            <td>
                <b>
                    Allow namespace to be omitted from URLs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposal to tweak our route generation so that namespaced routes will actually generate _two_ versions of the route:
* a base route like `/data` that implies use of the default namespace
* a namespaced route like `/namespaces/{ns}/data` that allows you to specify the namespace

To reduce clutter on the Swagger UI page, routes will also now be grouped into 3 category buckets. I'm open to names for these categories, but I've proposed "Global", "Default Namespace", and "Non-Default Namespace".

The main functional changes are in `internal/apiserver/routes.go`.

---

<img width="1852" alt="Swagger_UI" src="https://user-images.githubusercontent.com/1993829/166966999-5204cbf8-92d9-4762-9038-fd5ea21f4562.png">

---

<img width="1849" alt="Swagger_UI" src="https://user-images.githubusercontent.com/1993829/166967145-f1331a45-b5a9-44c6-8bb4-81ff0775fd21.png">

---

<img width="1847" alt="Swagger_UI" src="https://user-images.githubusercontent.com/1993829/166967227-0d996e36-4474-48f0-9ee9-5dec105b9f17.png">

---

<img width="1851" alt="Swagger_UI" src="https://user-images.githubusercontent.com/1993829/166967307-12ad9f93-1fcf-4f42-a5ba-435fbf0c0e75.png">
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 20:04:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/791" class=".btn">#791</a>
            </td>
            <td>
                <b>
                    Refactor to move common utility code out to firefly-common
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Moves base `pkg/fftypes` (time, numeric, bytes etc.) out to `firefly-common`
- Moves all FireFly Core data types from `pkg/fftypes` to `pkg/core`
- Removes the following packages that all moved to `firefly-common`:
  - `pkg/config`
  - `pkg/ffresty`
  - `pkg/httpserver`
  - `pkg/i18n`
  - `pkg/log`
  - `pkg/retry`
  - `pkg/wsclient`
- Only functional change: `api.shutdownTimeout` moved to be consistent with the other `httpserver` config, so is now split into three separate configurations:
   - `api.shutdownTimeout`
   - `admin.shutdownTimeout`
   - `metrics.shutdownTimeout`
- I decided to keep `cors.` as a global config shared across `api`/`admin`/`metrics` - which means initializing the HTTP Server now passes in two separate config prefixes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 19:44:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/790" class=".btn">#790</a>
            </td>
            <td>
                <b>
                    Split definition methods out of Broadcast Manager into new Definition Sender
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not totally crazy about the names `defsender.Sender` and `defhandler.DefinitionHandler`, but they need to be separate packages and this is where I landed...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 15:37:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/789" class=".btn">#789</a>
            </td>
            <td>
                <b>
                    Remove non-definition items from DefinitionHandler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #614
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 18:49:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/786" class=".btn">#786</a>
            </td>
            <td>
                <b>
                    update init logging branding
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
        Created At 2022-05-03 16:02:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/785" class=".btn">#785</a>
            </td>
            <td>
                <b>
                    update cobra short and long descriptions
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
        Created At 2022-05-03 13:28:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/784" class=".btn">#784</a>
            </td>
            <td>
                <b>
                    Adde custom onchain logic docs for Fabric plus refactoring
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
        Created At 2022-05-02 22:06:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/782" class=".btn">#782</a>
            </td>
            <td>
                <b>
                    Default for token approvals should be "approved: true"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 18:44:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/781" class=".btn">#781</a>
            </td>
            <td>
                <b>
                    Update manifest.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 13:07:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/780" class=".btn">#780</a>
            </td>
            <td>
                <b>
                    Token transfer/approval protocolId should be unique for each connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-01 18:14:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/778" class=".btn">#778</a>
            </td>
            <td>
                <b>
                    Fix bugs with token approvals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 18:46:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/777" class=".btn">#777</a>
            </td>
            <td>
                <b>
                    Update Tokens Tutorials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                This PR adds two brand new tutorials for ERC-20 and ERC-721 as well as how to use Metamask with them. It also includes some updates to the ERC-1155 tutorial to include approvals.

A live preview of the new docs pages can be found at: https://nguyer.github.io/firefly/tutorials/tokens
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 17:02:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/776" class=".btn">#776</a>
            </td>
            <td>
                <b>
                    [ui-v1.0.1] manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 15:43:57 +0000 UTC
    </div>
</div>

