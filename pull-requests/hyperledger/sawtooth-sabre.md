---
layout: default
title: sawtooth-sabre
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sabre
---

# sawtooth-sabre <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sabre){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/170" class=".btn">#170</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-5: Fix mistune doc build error
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
        Created At 2021-12-15 20:30:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-7: Fix mistune doc build error
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
        Created At 2021-12-15 20:30:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Fix mistune doc build error
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
        Created At 2021-12-15 16:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sabre/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    Switch simple logger to use UTC timestamps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates simple logger to be configured with UTC timestamps. Local timestamps require a compiler flag, unsound_local_offset, which is required by a transient dependency.  The time crate (the transient
dependency in question) describes this flag as untested, and it fails in certain environments, such as CI.

See https://time-rs.github.io/internal-api/time/index.html#feature-flags for more information

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 15:19:20 +0000 UTC
    </div>
</div>

