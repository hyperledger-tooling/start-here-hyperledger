---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    Update Java binding build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix errors and warnings from maven publish, i.e.

```
Repository "orghyperledger-1045" failures
  Rule "sources-staging" failures
   * Missing: no sources jar found in folder '/org/hyperledger/fabric/fabric-protos/0.1.2'
  Rule "javadoc-staging" failures
   * Missing: no javadoc jar found in folder '/org/hyperledger/fabric/fabric-protos/0.1.2'
```

and

```
'build.plugins.plugin.version' for org.apache.maven.plugins:maven-gpg-plugin is missing.
```

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 14:58:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Bump version to 0.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 11:54:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    Only tag release versions as latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The node module should only be tagged with “latest” for released versions, and “unstable” otherwise

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 11:49:42 +0000 UTC
    </div>
</div>

