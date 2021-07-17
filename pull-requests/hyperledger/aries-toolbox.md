---
layout: default
title: aries-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-toolbox
---

# aries-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/224" class=".btn">#224</a>
            </td>
            <td>
                <b>
                    Docs/admin credential definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 20:55:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/221" class=".btn">#221</a>
            </td>
            <td>
                <b>
                    docs: add docs for admin-schemas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Credit to @cjhowland for her work on this (originally written in a hackmd doc).

To generate new docs for protocols, first create a directory structure matching the following template: `admin-PROTOCOLHERE/VERSIONHERE`.

For example, for the schema admin protocol: `admin-schemas/0.1`.

Then, create a new `README.md` file in that directory. Populate this file with protocol documentation. The folder generator looks for specific lines in the file to generate folders from. There must be a line matching:

```
## Protocol Messages
```

(This line can have one or more `#` at the front)

This line is to be followed by lines matching the following template:

```
- [message-type](#message-type-section-title-in-doc)
```

For example:
```
#### Protocol Messages
* [send-schema](#send-schema)
* [schema-id](#schema-id)
...
```
In this case, the link and the link text match but the `#send-schema` is derived from the `### Send schema` header (markdown parsing on github turns headers into anchors on the web page by `to_lower`ing it and replacing spaces with hyphens)

To generate the folders after placing the `README.md` in the correct location, run:

```
make clean docs
```

From the `docs` folder.

This requires `make` and `awk` to be installed on your system. If you don't have these on your system, maintainers of this repository can take care of doc generation on your behalf.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 18:28:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-toolbox/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    Feature/schema input pattern
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 22:04:37 +0000 UTC
    </div>
</div>

