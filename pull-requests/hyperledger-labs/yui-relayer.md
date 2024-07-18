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
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    fix slog source attribute
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Problem:
RelayerLogger has wrapper functions to slog.log such as RelayerLogger.Error.
In case of application calls RelayerLogger.Error function, the source property of output log signs to RelayerLogger.Error function not caller of it.

# Resolve
Passing upper of call stack to slog.
To perform it, I need to directly call `slog.Handler().Handle(ctx, record)` function.

# others
Add test.
To simplify testing, I add writer paramerter to RelayerLog constructor.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 10:01:09 +0000 UTC
    </div>
</div>

