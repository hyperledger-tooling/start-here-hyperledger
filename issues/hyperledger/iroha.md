---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4511" class=".btn">4511</a>
            </td>
            <td>
                <b>
                    Rename `Upgrade::new` into `Upgrade::executor`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2-dev</span><span class="chip">api-changes</span>
            </td>
            <td>
                `Upgrade::new` is very vague. Either rename it into `Upgrade::executor` or `UpgradeExecutor::new`.
The assumption here is that there will be other things to upgrade, not only executor. Is this correct?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 06:18:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4499" class=".btn">4499</a>
            </td>
            <td>
                <b>
                    Investigate why `actions/setup-python@v5` fails sometimes in `I2::CI::check_for_incorrect_images`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2-dev</span><span class="chip">CI</span>
            </td>
            <td>
                The `I2::CI::check_for_incorrect_images` job fails sometimes with the following:

```
Error: The version '3.11' with architecture 'x64' was not found for this operating system.
```

[Example log](https://github.com/hyperledger/iroha/actions/runs/8796269117/job/24138820362#step:2:270)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 10:06:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4487" class=".btn">4487</a>
            </td>
            <td>
                <b>
                    Detect color support in `parity_scale_decoder`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2-dev</span>
            </td>
            <td>
                > Instead of feature-gating it, I would suggest following the same pattern that `iroha` (crate in /cli/) itself follows:
> 
> * It detects colors support automatically via `supports_color` crate
> * User can override it by `--terminal-colors=false`/`--terminal-colors=true` flag

_Originally posted by @0x009922 in https://github.com/hyperledger/iroha/pull/4486#discussion_r1572274579_
            
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-19 13:26:20 +0000 UTC
    </div>
</div>

