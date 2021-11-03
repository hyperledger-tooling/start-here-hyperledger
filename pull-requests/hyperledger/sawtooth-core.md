---
layout: default
title: sawtooth-core
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-core
---

# sawtooth-core <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-core){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2406" class=".btn">#2406</a>
            </td>
            <td>
                <b>
                    BACKPORT 1-2: Fix doc build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 6.0 release of PyYAML (a bandit dependency) introduced a change that
requires the `Loader=` argument when using `yaml.load()`. Because we don't need
any of the additional funcationality available in `yaml.load()`, this function
was switched to `yaml.safe_load()` instead.

https://github.com/yaml/pyyaml/pull/561

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 22:23:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2405" class=".btn">#2405</a>
            </td>
            <td>
                <b>
                    BACKPORT 1-3: Fix doc build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 6.0 release of PyYAML (a bandit dependency) introduced a change that
requires the `Loader=` argument when using `yaml.load()`. Because we don't need
any of the additional funcationality available in `yaml.load()`, this function
was switched to `yaml.safe_load()` instead.

https://github.com/yaml/pyyaml/pull/561

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 22:22:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2404" class=".btn">#2404</a>
            </td>
            <td>
                <b>
                    Fix doc build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 6.0 release of PyYAML (a bandit dependency) introduced a change that
requires the `Loader=` argument when using `yaml.load()`. Because we don't need
any of the additional funcationality available in `yaml.load()`, this function
was switched to `yaml.safe_load()` instead.

https://github.com/yaml/pyyaml/pull/561

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 18:35:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2403" class=".btn">#2403</a>
            </td>
            <td>
                <b>
                    Add batch status subcommand to to sawadm CLI
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
        Created At 2021-11-01 19:11:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2402" class=".btn">#2402</a>
            </td>
            <td>
                <b>
                    Add batch show subcommand to sawadm CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 21:08:37 +0000 UTC
    </div>
</div>

