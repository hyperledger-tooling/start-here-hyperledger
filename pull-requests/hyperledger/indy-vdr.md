---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    fix(js): cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Renamed all packages to prefix `indy-vdr-`
  - This was done as there were issues with an example application when a folder in the workplace is called `react-native`. This is quite explicit, but it would fix some annoying IDE error and linting warnings.
- Removed some scripts as we do most stuff from the root at `wrapper/javascript`


Work funded by the Government of Ontario.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 12:49:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    build(iOS): add CI/CD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds the build pipeline for the iOS libraries
- Creates an xcframework 

It does not really integrate well with the current way to release the libraries. Do we want to build everything but just not add the artefacts for pull requests?

---

I also disabled LTO as it was causing issues when building a static library required for iOS. I am not too sure what the issue exactly is, but the symbols that are present in the dylib are not exposed.

```bash
# with LTO
indy-vdr λ nm target/release/libindy_vdr.a 2> /dev/null | rg _indy_vdr | wc -l
      0
# without LTO
indy-vdr λ nm target/release/libindy_vdr.a 2> /dev/null | rg _indy_vdr | wc -l
      44
```

Work funded by the Government of Ontario.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 14:57:54 +0000 UTC
    </div>
</div>

