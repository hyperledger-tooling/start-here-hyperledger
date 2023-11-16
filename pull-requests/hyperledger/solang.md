---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1596" class=".btn">#1596</a>
            </td>
            <td>
                <b>
                    Move LoopScopes into ExprContext
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This simplifies the code, and makes it to use ExprContext for other purposes (for example variable scoping).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 12:23:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1595" class=".btn">#1595</a>
            </td>
            <td>
                <b>
                    Add a feature flag for the language server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The language server alone pulls over 200 dependencies, or close to half of our total dependencies. Currently, `cargo build` causes to compile 552 crates. With this feature flag, a `cargo build --no-default-features --features llvm,wasm_opt` compiles only 296 crates.

And there are some chunky ones in the language server too. With the LS I get the following timings:

|Rank| Unit | Total | Codegen | Features
|-- | -- | -- | -- | --
|1. | wasm-opt-sys v0.112.0 build script (run) | 50.1s |   |  
|2. | **ethers-solc v2.0.10** | 16.0s | 7.1s (45%) | async, futures-util, sha2, svm, svm-builds, svm-solc
|3. | solang v0.3.3 bin "solang" | 15.8s |   | contract-build, default, ethers-core, forge-fmt, inkwell,  language_server, libc, llvm, rust-lapper, tokio, tower-lsp, wasm-opt,  wasm_opt
|4. | solang-parser v0.3.3 build script (run) | 13.8s |   | default
|5. | solang-parser v0.3.2 build script (run) | 13.4s |   | default
|6. | **lsp-types v0.94.1** | 9.9s | 1.1s (11%) | default
|7. | **ethers-core v2.0.10** | 8.1s | 3.5s (43%) |  
|8. | lalrpop v0.20.0 | 7.9s | 3.1s (39%) |  
|9. | **tokio v1.34.0** | 7.1s | 3.6s (51%) | bytes, default, fs, io-std, io-util, libc, macros, mio, net,  num_cpus, process, rt, rt-multi-thread, signal-hook-registry, socket2,  sync, time, tokio-macros
|10. | solang v0.3.3 | 6.5s | 2.4s (38%) | contract-build, default, ethers-core, forge-fmt, inkwell,  language_server, libc, llvm, rust-lapper, tokio, tower-lsp, wasm-opt,  wasm_opt
|11. | syn v1.0.109 | 6.2s | 2.6s (41%) | clone-impls, default, derive, extra-traits, fold, full, parsing, printing, proc-macro, quote, visit, visit-mut
|12. | **foundry-config v0.2.0** | 6.2s | 4.1s (66%) | 


Main offender is still `wasm-opt` by far, but we already have a flag for this.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-14 10:25:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1593" class=".btn">#1593</a>
            </td>
            <td>
                <b>
                    Parse pragma solidity version numbers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Many Solidity features depend on the version of the compiler. So, parse the version pragma and in another PR we will use this information.

This PR adds pragmas to the ast and we test it with a graphviz dot file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 16:32:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1592" class=".btn">#1592</a>
            </td>
            <td>
                <b>
                    Improve overloaded function call diagnostics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes: https://github.com/hyperledger/solang/issues/1534
Fixes: https://github.com/hyperledger/solang/issues/707
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-10 09:15:26 +0000 UTC
    </div>
</div>

