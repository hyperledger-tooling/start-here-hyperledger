---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2432" class=".btn">#2432</a>
            </td>
            <td>
                <b>
                    fix ordering of attributes being used before being introduced
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Axel Nennker <axel.nennker@telekom.de>

The compiler was complaining about the following:

> warning: derive helper attribute is used before it is introduced
   --> src/services/pool/types.rs:357:3
    |
357 | #[serde(tag = "op")]
    |   ^^^^^
358 | #[derive(Serialize, Deserialize, Debug)]
    |          --------- the attribute is introduced here
    |
    = warning: this was previously accepted by the compiler but is being phased out; it will become a hard error in a future release!
    = note: for more information, see issue #79202 <https://github.com/rust-lang/rust/issues/79202>


This PR reorders the two code lines so that the attribute is used after being introduced

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 14:23:50 +0000 UTC
    </div>
</div>

