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
                This is a proof of concept - only implemented for one route, and probably not as clean as it could be. Essentially the proposal is to tweak our route generation so that namespaced routes will actually generate _two_ versions of the route:
* a base route like `/data` that implies use of the default namespace
* a namespaced route like `/namespaces/{ns}/data` that allows you to specify the namespace

---

<img width="1724" alt="Swagger_UI" src="https://user-images.githubusercontent.com/1993829/166816835-b944d674-d46e-469c-a560-3f45361ffc8f.png">

---

<img width="1633" alt="Swagger_UI" src="https://user-images.githubusercontent.com/1993829/166816904-2742a7fb-c7b8-442f-bd0b-cdba6eb76946.png">
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
                PR <a href="https://github.com/hyperledger/firefly/pull/783" class=".btn">#783</a>
            </td>
            <td>
                <b>
                    Fix link to contributing documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Problem

404 when clicking on link to contributing docs.

# Action

Fix url in `CONTRIBUTING.md`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 20:30:43 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/775" class=".btn">#775</a>
            </td>
            <td>
                <b>
                    Clean up API spec for token approvals
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
        Created At 2022-04-28 20:56:54 +0000 UTC
    </div>
</div>

