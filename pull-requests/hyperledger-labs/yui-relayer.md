---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    add `ChainInfo::Timestamp` and implement it for the tendermint chain module
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
        Created At 2023-08-24 08:10:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    Add OTel metrics
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
        Created At 2023-08-21 13:14:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    Add path config edit command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add edit command to config commands
```
$RELAY paths edit $PATH_NAME [key] [src/dst] [value]
```
example
```
$RLY paths edit $PATH_NAME src client-id clinet-id-src
$RLY paths edit $PATH_NAME dst client-id clinet-id-dst

$RLY paths edit $PATH_NAME src connection-id connection-id-src
$RLY paths edit $PATH_NAME dst connection-id connection-id-dst

$RLY paths edit $PATH_NAME src channel-id channel-id-src
$RLY paths edit $PATH_NAME dst channel-id channel-id-dst

$RLY paths edit $PATH_NAME src port-id port-id-src
$RLY paths edit $PATH_NAME dst port-id port-id-dst

$RLY paths edit $PATH_NAME aaa port-id port-id-dst
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 08:13:35 +0000 UTC
    </div>
</div>

