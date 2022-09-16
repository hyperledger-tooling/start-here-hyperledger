---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2159" class=".btn">#2159</a>
            </td>
            <td>
                <b>
                    fix(plugin-keychain-vault): hyper upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
--------------------------------

fix(plugin-keychain-vault): hyper upgrade   

    Primary changes
    --------------
    1. Updated rust docker container base image to the latest
    2. Updated hyper, hyper-openssl, hyper-tls, swagger, tokio, tokio-openssl versions in cargo.toml
    3. Updated the depricated to_body() method to to_bytes() method and relevant imports

Fixes #2120

Signed-off-by: jagpreetsinghsasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 07:33:20 +0000 UTC
    </div>
</div>

