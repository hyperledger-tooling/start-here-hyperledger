---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/389" class=".btn">#389</a>
            </td>
            <td>
                <b>
                    Upgrade wawaka to WAMR-1.1.2 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Key new features since last supported version (WAMR-01-19-2022):

- Since [WAMR-05-18-2022](https://github.com/bytecodealliance/wasm-micro-runtime/releases/tag/WAMR-05-18-2022)
  * Implement Berkeley Socket APIs for libc-wasi and linux-sgx platforms
  * Fix native stack overflow check failed in interpreter
  * Fix various AOT compilation and loader issues

- Since [fast-jit-06-29-2022](https://github.com/bytecodealliance/wasm-micro-runtime/releases/tag/fast-jit-06-29-2022):
  * First implementation of fast JIT

- Since [WAMR-1.0.0](https://github.com/bytecodealliance/wasm-micro-runtime/releases/tag/WAMR-1.0.0)
  * Implement HW bound check for interpreter and Fast JIT
  * Implement Python and go language bindings
  * Enable SGX remote attestation using librats
  * Add a new API to get free memory in memory pool
  * Enable AOT compiler with llvm-14/15
  * Support 3rd-party toolchains in wamrc

- Since [WAMR-1.1.0](https://github.com/bytecodealliance/wasm-micro-runtime/releases/tag/WAMR-1.1.0)
  * Add support for SGX IPFS
  * Add check for code section size, fix interpreter float operations
  * Prevent an already detached thread from being detached again for thread manager

- Since [WAMR-1.1.1](https://github.com/bytecodealliance/wasm-micro-runtime/releases/tag/WAMR-1.1.1)
  * Improvements to Socket API implementations
  * Integrate WASI-NN into WAMR: support TensorFlow/CPU/F32 in the first stage

- Since [WAMR-1.1.2](https://github.com/bytecodealliance/wasm-micro-runtime/releases/tag/WAMR-1.1.2)
  * Change iwasm exit code in certain conditions
  * Enable bulk memory by default; normalize how the global heap pool is configured across iwasm apps
  * Refine AOT exception checks when functions return
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 22:55:53 +0000 UTC
    </div>
</div>

