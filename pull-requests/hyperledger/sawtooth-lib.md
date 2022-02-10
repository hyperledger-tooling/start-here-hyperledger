---
layout: default
title: sawtooth-lib
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-lib
---

# sawtooth-lib <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-lib){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    Update and patch transact version to 0.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit updates the transact version to be 0.5.
This version is not yet released but will be the
version used in the 0.8 (current main) release of
libsawtooth. As such, a patch is added into the Cargo.toml
to have the transact version be pulled in from the main
branch of transact on github.

This is required before https://github.com/Cargill/splinter/pull/1801 will work
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 19:11:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-6: Set dotenv-load to true in justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Starting with version 0.11.0, just ignores .env files by default. This
breaks some recipes because we read docker environment variables from
the .env file.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 15:05:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-7: Set dotenv-load to true in justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Starting with version 0.11.0, just ignores .env files by default. This
breaks some recipes because we read docker environment variables from
the .env file.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 15:05:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-lib/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    Set dotenv-load to true in justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Starting with version 0.11.0, just ignores .env files by default. This
breaks some recipes because we read docker environment variables from
the .env file.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 15:35:23 +0000 UTC
    </div>
</div>

