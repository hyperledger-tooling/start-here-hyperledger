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
                Issue <a href="https://github.com/hyperledger/iroha/issues/4704" class=".btn">4704</a>
            </td>
            <td>
                <b>
                    Implement `Instruction` for `*Box` wrappers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span>
            </td>
            <td>
                Currently, only `InstructionBox` implements `Instruction` out of all ISI wrappers. I expected `RegisterBox`, `MintBox` and the rest of the wrappers to be usable with `iroha.submit_*()` directly, but they are not. I think it would be more ergonomic if they were.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 11:42:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4703" class=".btn">4703</a>
            </td>
            <td>
                <b>
                    remove `Sealed` trait from `Instruction` supertraits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                > To use `client.submit()` for `CustomInstructionExpr`, it is necessary for `CustomInstructionExpr` to implement `Instruction` and `Sealed` traits. This will require some changes to iroha_data_model (at least make `Sealed` trait public). I am not sure if it is worth it.
> 
> Currently I added `pub fn into_instruction(self) -> InstructionBox` method to `CustomInstructionExpr`, so it is possible to write:
> 
> ```rust
> let isi = CustomInstructionExpr::If(...);
> client.submit_blocking(isi.into_instruction())?;
> ```

_Originally posted by @dima74 in https://github.com/hyperledger/iroha/pull/4645#discussion_r1626440158_
            
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 11:20:08 +0000 UTC
    </div>
</div>

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

