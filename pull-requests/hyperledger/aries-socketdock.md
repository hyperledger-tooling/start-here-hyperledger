---
layout: default
title: aries-socketdock
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-socketdock
---

# aries-socketdock <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-socketdock){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-socketdock/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    refactor: refine socketdock
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a refinement of the socketdock server:

- Add pre-commit config files
- Use slim-bullseye image
- Make command line arguments a bit more conventional (`-` instead of `_`, `--endpoint` instead of `externalhostandport`)
- Structure the project as a python package, moving main entrypoint to `socketdock/__main__.py`
- Move API logic to it's own "blueprint" module
- Use `ContextVar`s for simple dependency inversion
- Docstrings everywhere
- Handle some cases where undefined variables or incompatible data types were possible
- Make `Backend` officially an ABC
- Better error handling in HTTP Backend
- Module scoped loggers instead of using the global logging interface
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-15 02:16:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-socketdock/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    ci: add image publish workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a GHA for publishing an image for this project. The image publish is triggered on release or manually.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-15 00:54:52 +0000 UTC
    </div>
</div>

