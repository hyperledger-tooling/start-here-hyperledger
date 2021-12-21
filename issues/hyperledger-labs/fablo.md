---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/fablo/issues/265" class=".btn">265</a>
            </td>
            <td>
                <b>
                    Change CouchDB image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span>
            </td>
            <td>
                Currently for CouchDB we are using images provided by Hyperledger. It's not good option anymore because:

1. It's deprecated: https://github.com/hyperledger/fabric/releases
```
Fabric CouchDB image is deprecated
v2.2.0 added support for CouchDB 3.1.0 as the recommended and tested version of CouchDB.
If prior versions are utilized, a Warning will appear in peer log.
Note that CouchDB 3.1.0 requires that an admin username and password be set, while this was optional in CouchDB v2.x. See the Fabric CouchDB documentation for configuration details.
Also note that CouchDB 3.1.0 default max_document_size is reduced to 8MB. Set a higher value if needed in your environment.
Finally, the fabric-couchdb docker image will not be updated to v3.1.0 and will no longer be updated, maintained, or published.
Users can utilize the official CouchDB docker image maintained by the Apache CouchDB project instead.
```

2. Seems that it doesn't work in some setups: https://github.com/hyperledger-labs/fablo/issues/263
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 10:44:46 +0000 UTC
    </div>
</div>

