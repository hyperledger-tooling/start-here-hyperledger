---
layout: default
title: firefly-perf-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-perf-cli
---

# firefly-perf-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-perf-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    New run Command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Provides a YAML or JSON "DSL" for defining multiple test "instances". A test instance consists of a _single_ test type, test options, length, and number of workers.

The idea is that we can now run multiple instances of `ffperf` either with `nohup` or multiple containers / pods. Each instance just then takes in a different `--instance-name` or `--instance-index` to determine what it runs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 18:32:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Add broadcast and private blob transfer perf tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly-perf-cli/issues/21
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 14:42:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Cleaning up prep.sh after ffperf
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
        Created At 2022-03-17 20:38:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Renaming to ffperf with run-tests and version Subcommands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Renames from `ff-perf` to `ffperf`
* Moves root command functionality to `run-tests` subcommand so folks can continue running / adding new tests while the first draft of the `run-instance` command is implemented, see https://discord.com/channels/905194001349627914/928377875827154984/953668508196175912 for more details
* Adds `version` subcommand for future gorelease builds and to serve as additional output from perf tests
* Adds `Makefile` and `.goreleaser.yaml` for easier building of gitignored binaries and fixing GHA builds

Example uses locally w/o a real FF env thats up:
```
./dist/firefly-perf-cli_darwin_arm64/ffperf version
{
  "Version": "v0.0.1-next",
  "Commit": "3318bad025b90f1b58744626c884eb76d2b120d5",
  "Date": "2022-03-17T19:47:18Z",
  "License": "Apache-2.0"
}

./dist/firefly-perf-cli_darwin_arm64/ffperf run-tests msg_broadcast -l 500h -w 10
INFO[2022-03-17T15:49:55.909] Created subscription on http://localhost:5000: perf_db5b34f0-77d2-4b51-a345-07b56715792a 
WARN[2022-03-17T15:49:55.911] WS ws://localhost:5000/ws connect attempt 1 failed [403]:  
WARN[2022-03-17T15:49:56.166] WS ws://localhost:5000/ws connect attempt 2 failed [403]:  
WARN[2022-03-17T15:49:56.670] WS ws://localhost:5000/ws connect attempt 3 failed [403]:  
WARN[2022-03-17T15:49:57.676] WS ws://localhost:5000/ws connect attempt 4 failed [403]:  
WARN[2022-03-17T15:49:59.680] WS ws://localhost:5000/ws connect attempt 5 failed [403]: 
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 19:53:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Add Fabric custom contract test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 18:13:32 +0000 UTC
    </div>
</div>

