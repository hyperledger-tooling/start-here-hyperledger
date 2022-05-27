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
                PR <a href="https://github.com/hyperledger/firefly/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    set message header type for broadcast/private
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                FireFly now sets the message type for any broadcast or private messages
sent via the API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 18:12:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/837" class=".btn">#837</a>
            </td>
            <td>
                <b>
                    Use firefly-signer library and allow numbers expressed as strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR introduces `firefly-signer`'s ABI parsing functions and uses them in FireFly's ABI -> FFI generation code. It also replaces any existing ABI data structures that were originally copied over from Ethconnect, with those of `firefly-signer`.

This PR also makes some enhancements to the ABI -> FFI generation code itself to allow numbers to be expressed in a JSON string or a JSON number. This is reflected in the generated OpenAPI Spec for custom contracts, including a description in the Swagger UI that describes this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 17:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/836" class=".btn">#836</a>
            </td>
            <td>
                <b>
                    default fabconnect calls to async
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                The fabconnect default for `/transactions` is synchronous. The fabric plugin currently expects async responses, so adding the `x-firefly-sync` header.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 17:27:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/835" class=".btn">#835</a>
            </td>
            <td>
                <b>
                    Update README with missing links, and bit of a restructure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I found a few links were missing, and given how many repos we've grown to I proposed a bit of organization too.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 03:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/834" class=".btn">#834</a>
            </td>
            <td>
                <b>
                    Backport docs generation and versioning code for 1.0 stream
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR backports several things into the 1.0 release stream for generating new docs pages going forward:

- Structural changes to the docs site, including embedding the theme
- The new GitHub action which builds and publishes docs versions
- The new docs internationalization support
- The new Go code to generate reference docs pages
- All the description includes for reference types

There is no new code in this PR. Just porting over existing code from `main` onto the `release-1.0` branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 17:04:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/833" class=".btn">#833</a>
            </td>
            <td>
                <b>
                    Namespace config validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding additional configuration validation to the namespace manager, as specified in [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)


* `name` must be unique on this node
 * for historical reasons, "ff_system" is a reserved string and cannot be used as a `name` or `remoteName`
 * a `database` plugin is required for every namespace
 * if `mode: multiparty` is specified, plugins _must_ include one each of `blockchain`,
  `dataexchange`, and `sharedstorage`
 * if `mode: gateway` is speicified, plugins _must not_ include `dataexchange` or `sharedstorage`
 * at most one of each type of plugin is allowed per namespace, except for tokens (which
  may have many per namespace)

depends on changes in https://github.com/hyperledger/firefly-common/pull/14
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 15:42:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/832" class=".btn">#832</a>
            </td>
            <td>
                <b>
                    Fix relative links in reference descriptions docs
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
        Created At 2022-05-24 15:26:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/831" class=".btn">#831</a>
            </td>
            <td>
                <b>
                    Fix link to events reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 21:04:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    Add version support to docs site
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds significant new functionality to the docs GitHub action to manage versions of the docs site. This will create a directory tree that ends up looking like this:

```
+ / (latest release)
|-- v1.0.0
|-- v1.0.1
|-- ...
|-- head (current commit in main)
```

It will also build a JSON file that contains the full list of all these versions to build the dropdown menu that shows up in the docs rendered pages (with the addition of a `latest` link that links to `/`).

These changes allow us to always keep the docs up to date with the code in the same commit, but users navigating to the docs site will see the latest release by default. They can also use the dropdown menu to browse older release as well.

> **NOTE** There will be a one time manual action necessary to generate docs for older versions. I can take care of this after this PR is approved and merged.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 20:06:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    Possible to see clash on port 6000 for metrics server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Saw a build failure in https://github.com/hyperledger/firefly/runs/6530517574?check_suite_focus=true

```
Error: FF00151: Unable to start listener on 127.0.0.1:6000: %!s(MISSING): listen tcp 127.0.0.1:6000: bind: address already in use
```

We have config to get a dynamically assigned port for these tests for `debug` and `http`, but not for `metrics`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 13:04:41 +0000 UTC
    </div>
</div>

