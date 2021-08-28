---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1275" class=".btn">#1275</a>
            </td>
            <td>
                <b>
                    feat(odap): odap first pr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The first pull request for odap

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 04:30:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1274" class=".btn">#1274</a>
            </td>
            <td>
                <b>
                    feat(tools): substrate test ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Substrate-based blockchains like Polkadot are becoming increasingly relevant. However, Cactus does not have tools to support developing Substrate-based connectors, such as a test ledger.


This draft PR provides a first attempt at defining a Substrate test ledger, that allows to programmatically instantiate the Substrate node template (https://github.com/substrate-developer-hub/substrate-node-template).
Thus, it contains a Dockerfile with the test ledger and the test-ledger file that contains the execution logic.

I would appreciate feedback on the tools/docker/substrate-all-in-one/Dockerfile and packages/cactus-test-tooling/src/main/typescript/substrate-test-ledger/substrate-test-ledger.ts files prior to merging.


Notes:
At the moment a bug occurs in the Dockerfile at RUN   rustup update nightly


info: syncing channel updates for 'nightly-x86_64-unknown-linux-gnu'
info: latest update on 2021-08-26, rust version 1.56.0-nightly (0afc20860 2021-08-25)
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: downloading component 'cargo'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: removing previous version of component 'rust-std' for 'wasm32-unknown-unknown'
info: rolling back changes
error: could not rename component file from '/usr/local/rustup/toolchains/nightly-x86_64-unknown-linux-gnu/lib/rustlib/wasm32-unknown-unknown/lib' to '/usr/local/rustup/tmp/jxirtjwr7gf70a8r_dir/bk'
error: caused by: other os error
error: backtrace:
error:    0: error_chain::backtrace::imp::InternalBacktrace::new
   1: rustup::utils::utils::rename
   2: rustup::dist::component::transaction::Transaction::remove_dir
   3: rustup::dist::component::components::Component::uninstall
   4: rustup::dist::manifestation::Manifestation::update
   5: rustup::dist::dist::update_from_dist_
   6: rustup::install::InstallMethod::install
   7: rustup::toolchain::DistributableToolchain::install_from_dist
   8: rustup::cli::rustup_mode::update
   9: rustup::cli::rustup_mode::main
  10: rustup_init::main
  11: std::rt::lang_start_internal::{{closure}}::{{closure}}
             at rustc/c7087fe00d2ba919df1d813c040a5d47e43b0fe7/src/libstd/rt.rs:52
      std::sys_common::backtrace::__rust_begin_short_backtrace
             at rustc/c7087fe00d2ba919df1d813c040a5d47e43b0fe7/src/libstd/sys_common/backtrace.rs:130
  12: main
  13: __libc_start_main
  14: <unknown>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 02:46:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1273" class=".btn">#1273</a>
            </td>
            <td>
                <b>
                    fix(config): remove no longer working scripts from package.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes: #1271
Signed-off-by: Michael Courtin <michael.courtin@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 13:31:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1270" class=".btn">#1270</a>
            </td>
            <td>
                <b>
                    build(dev-container): fix yarn not found error #1269
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Primary change:
------------------

The post-create-command.sh script will now run the
install-yarn script prior to calling the configure script.
This wil lensure that yarn is installed by the time the
configure script is invoked.

Secondary change(s):
------------------------

Applied automatic formatting to the Dockerfile and the
aforementioned post-create-commands script as well.

Fixes #1269

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 17:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1268" class=".btn">#1268</a>
            </td>
            <td>
                <b>
                    refactor(cmd-server-socket,validator): [draft] refactor the directory structure of cmd-server-socket and validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolving #1233 (work-in-progress)
- status: Draft

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 14:47:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    fix(indy-validator): fixing indy validator initialization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes issue #1266.

- Added initialization code before pool.open_pool_ledger API call.
- Also added a key file necessary for the server.

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 14:36:26 +0000 UTC
    </div>
</div>

