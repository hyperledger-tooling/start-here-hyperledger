---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    shrink unsafe block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this function you use the unsafe keyword for some safe expressions. However, I found that only 1 function are real unsafe operations (see the list below). 

We need to mark unsafe operations more precisely using unsafe keyword. Keeping unsafe blocks small can bring many benefits. For example, when mistakes happen, we can locate any errors related to memory safety  within an unsafe block. This is the balance between Safe and Unsafe Rust. The separation is designed to make using Safe Rust as ergonomic as possible, but requires extra effort and care when writing Unsafe Rust. 
**Real unsafe operation list:**
1. the from_raw() function(unsafe function)

Hope this PR can help you.
Best regards.
**References**
https://doc.rust-lang.org/nomicon/safe-unsafe-meaning.html 
https://doc.rust-lang.org/book/ch19-01-unsafe-rust.html 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 05:49:20 +0000 UTC
    </div>
</div>

