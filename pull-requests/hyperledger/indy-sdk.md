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
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2453" class=".btn">#2453</a>
            </td>
            <td>
                <b>
                    postgres_storage: Changed type in unsafe block to be able to compile on arm64 architecture 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @WadeBarnes thanks for the hint:  Replaced `*const i8` with `libc::c_char` in `unsafe {}` blocks in file `lib.rs` to be able to compile on linux/arm64 architecture. Now compiles on Ubuntu 20.04 aarch64 and MacOS 12.0.1 (Apple M1, arm64/v8). Rust Version: 1.56.0

`unsafe { *tags_json_ptr = record.tags.as_ptr() as *const libc::c_char; }`

*Deprecation Warnings*
Changed [deprecated use](https://blog.rust-lang.org/2020/03/12/Rust-1.42.html#errordescription-is-deprecated) of `err.description()` to silence warnings
`warning: use of deprecated item std::error::Error::description: use the Display impl or to_string()`
 in `src/common.rs, src/wallet.rs, src/crypto.rs`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 10:43:10 +0000 UTC
    </div>
</div>

