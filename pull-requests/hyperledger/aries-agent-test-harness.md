---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/693" class=".btn">#693</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 03:04:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/692" class=".btn">#692</a>
            </td>
            <td>
                <b>
                    GENESIS_URL Support for Connectionless proof request on and external ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds GENESIS_URL support to the test harness. You can now use GENESIS_URL instead of LEDGER_URL_CONFIG when running tests or starting agents as a service. There are currently no test run sets that use the GENESIS_URL. 

### Use Case
The BC Wallet tests in Aries Mobile Test Harness uses AATH agents as a service to accomplish Issuer and Verifier roles with the wallet app tests. Some tests are using an issuer that is on the CANdy network. There was a need to a verifier to do a connectionless proof request with a credential from that issuer. The verifier agent needed to be started with the GENESIS_URL from the CANdy network, and the agent is started in read only mode since it does not need(could not get) write access to the ledger. If read only mode is set, then the ACA-Py agent does not register a did on the network.

There is a new yaml file aries-backchannels/acapy/read_only_ledger_verifier_config.yaml that can be used if anyone wants to start an agent with read only ledger access and with all the auto responding turned on. 

This allows us to do a command as follows to accomplish the use case. 
```
GENESIS_URL=https://whatever.genesis.url.you.want AGENT_CONFIG_FILE=/aries-backchannels/acapy/read_only_ledger_verifier_config.yaml ./manage start -b acapy-main
```

### Other Enhancements
To support the GENESIS_URL above I also refactored how environment variables were gathered and sent to the test containers. There is no longer multiple conditional calls to docker run based on what env vars are set. There is now one call. 

The uniresolver was hardcoded to use the LEDGER_URL. It now will use the GENESIS_URL if it is set. 

### Considerations

- This works for the ACA-Py agent/backchannel. There may need to be work done in other backchannels if they wish to use the GENESIS_URL in their workflows. 

- I tested this with a bunch of different run commands that are used in the interop regression tests. All seemed to be fine since they set the LEDGER_URL_CONFIG in the workflows. However, I did try a run command with no LEDGER_URL or GENESIS_URL. My expectation was that it would start a local ledger, then use that in the tests however there was an issue running a command like this, 
```
./manage run -d acapy-main -t @AcceptanceTest -t @AIP20 -t ~@wip -t @T004-RFC0211
```
The genesis transaction was setup and the agent started but would throw this error. 
```
2023-06-05 18:54:30,258 aries_cloudagent.commands.start ERROR Exception during startup:
Traceback (most recent call last):
  File "/usr/local/lib/python3.7/site-packages/aries_cloudagent/commands/start.py", line 72, in init
    await startup
  File "/usr/local/lib/python3.7/site-packages/aries_cloudagent/commands/start.py", line 28, in start_app
    await conductor.setup()
  File "/usr/local/lib/python3.7/site-packages/aries_cloudagent/core/conductor.py", line 185, in setup
    self.root_profile, self.setup_public_did and self.setup_public_did.did
  File "/usr/local/lib/python3.7/site-packages/aries_cloudagent/config/ledger.py", line 136, in ledger_config
    async with ledger:
  File "/usr/local/lib/python3.7/site-packages/aries_cloudagent/ledger/indy.py", line 318, in __aenter__
    await self.pool.context_open()
  File "/usr/local/lib/python3.7/site-packages/aries_cloudagent/ledger/indy.py", line 239, in context_open
    await self.open()
  File "/usr/local/lib/python3.7/site-packages/aries_cloudagent/ledger/indy.py", line 204, in open
    self.handle = await indy.pool.open_pool_ledger(self.name, pool_config)
  File "/usr/local/lib/python3.7/site-packages/indy/pool.py", line 88, in open_pool_ledger
    open_pool_ledger.cb)
  File "/usr/local/lib/python3.7/asyncio/futures.py", line 263, in __await__
    yield self  # This tells Task to wait for completion.
  File "/usr/local/lib/python3.7/asyncio/tasks.py", line 318, in __wakeup
    future.result()
  File "/usr/local/lib/python3.7/asyncio/futures.py", line 176, in result
    raise CancelledError
concurrent.futures._base.CancelledError
2023-06-05 18:54:30,267 aries_cloudagent.indy.sdk.profile DEBUG Profile finalizer called; closing wallet
2023-06-05 18:54:30,324 asyncio ERROR Task exception was never retrieved
future: <Task finished coro=<run_loop.<locals>.done() done, defined at /usr/local/lib/python3.7/site-packages/aries_cloudagent/commands/start.py:77> exception=RuntimeError('cannot reuse already awaited coroutine')>
Traceback (most recent call last):
  File "/usr/local/lib/python3.7/asyncio/tasks.py", line 249, in __step
    result = coro.send(None)
RuntimeError: cannot reuse already awaited coroutine
```
I don't believe any of my changes would affect this and I ~~am assuming~~ have confirmed this issue existed before my changes. There are no workflows that use the test harness in this manner as far as I know, so it should not impact the interop regression test cycle.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 18:58:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/691" class=".btn">#691</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 03:11:31 +0000 UTC
    </div>
</div>

