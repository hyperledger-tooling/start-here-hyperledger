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
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    fix(js): defer library loading for nodejs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevent native library from being loaded right when `@hyperledger/indy-vdr-nodejs` is imported by deferring its loading to when it's actually used. 

This is a problem we found during AFJ test suites, which import the library in general purpose test helpers and make the native library to be loaded more times than needed, allocating more memory and making the suite to crash.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 16:50:59 +0000 UTC
    </div>
</div>

