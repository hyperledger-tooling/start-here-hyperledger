---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    Fix push of latest docker tag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since this is the last line in the action, this is probably the last fix that will be needed :disappointed: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 11:48:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Fix tagging of latest image on release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the current problem with tagging latest on a release build
```
Run docker tag ghcr.io/hyperledger/firefly-ethconnect:latest ghcr.io/hyperledger/firefly-ethconnect:latest
  docker tag ghcr.io/hyperledger/firefly-ethconnect:latest ghcr.io/hyperledger/firefly-ethconnect:latest
  shell: /usr/bin/bash -e {0}
Error response from daemon: No such image: ghcr.io/hyperledger/firefly-ethconnect:latest
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 20:21:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    Fix use of GITHUB_REF in docker build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Third time's the charm, right?

This should fix the fact that (despite what GitHub's documentation says) `GITHUB_REF` includes `refs/tags/` before the actual tag name. Using shell expansion, we can grab just the last part of the variable.

I tested the shell expansion locally and it seems to do the trick:
```
➜  ~ export GITHUB_REF="refs/tags/3.0.1"
➜  ~ echo $GITHUB_REF
refs/tags/3.0.1
➜  ~ echo ${GITHUB_REF##*/}
3.0.1
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 15:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    Update ref to latest ethbinding
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
        Created At 2021-10-11 20:14:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Fix docker release trigger
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
        Created At 2021-10-11 20:11:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    Avoid holding batchCond while dispatching updateInterrupt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In #162 there is the following deadlock:

### Deadlock investigation

Batch processor trying to notify eventPoller to stop using `updateInterrupt`:
```
goroutine 547 [chan receive]:
github.com/hyperledger/firefly-ethconnect/internal/events.(*eventStream).batchProcessor(0xc0001be160)
	/ethconnect/internal/events/eventstream.go:544 +0x11b
created by github.com/hyperledger/firefly-ethconnect/internal/events.(*eventStream).startEventHandlers
	/ethconnect/internal/events/eventstream.go:209 +0x10c
```
https://github.com/hyperledger/firefly-ethconnect/blob/d686811c70f27d063730660e411185095fe7da1b/internal/events/eventstream.go#L544

Event poller trying to obtain the `batchCond`:
```
goroutine 546 [semacquire]:
sync.runtime_SemacquireMutex(0xc000028334, 0xbc8800, 0x1)
	/usr/local/go/src/runtime/sema.go:71 +0x47
sync.(*Mutex).lockSlow(0xc000028330)
	/usr/local/go/src/sync/mutex.go:138 +0x105
sync.(*Mutex).Lock(0xc000028330)
	/usr/local/go/src/sync/mutex.go:81 +0x47
github.com/hyperledger/firefly-ethconnect/internal/events.(*eventStream).isBlocked(0xc0001be160, 0xc000292030)
	/ethconnect/internal/events/eventstream.go:356 +0x5c
github.com/hyperledger/firefly-ethconnect/internal/events.(*eventStream).eventPoller(0xc0001be160)
	/ethconnect/internal/events/eventstream.go:393 +0xd85
created by github.com/hyperledger/firefly-ethconnect/internal/events.(*eventStream).startEventHandlers
	/ethconnect/internal/events/eventstream.go:207 +0xcc
```
https://github.com/hyperledger/firefly-ethconnect/blob/d686811c70f27d063730660e411185095fe7da1b/internal/events/eventstream.go#L356
... called from this loop:
https://github.com/hyperledger/firefly-ethconnect/blob/d686811c70f27d063730660e411185095fe7da1b/internal/events/eventstream.go#L393
... which is where we would pull from the `updateInterrupt`

### Proposed fix

Release the `batchCond` lock, before consuming from the `updateInterrupt` channel
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 20:00:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/163" class=".btn">#163</a>
            </td>
            <td>
                <b>
                    Create tagged image when publishing a release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This GitHub action change should add an additional tag to the docker image when a new release is published. The image will be tagged with whatever the name of the release is. This will also update the `latest` image to point to the newest release.

> Note: after this merge, we will no longer be building new docker images on merges to `main`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 18:23:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    Make requestABIId omitempty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Two small observations in e2e testing of #159 fix:
- `requestABIId` does not have `omitempty`
  - Change made here
-  Would be helpful to fill this in, for the case we generated the ABI ID from the request ID, to make it clear we did that
  - This is actually really hard, due to where it's assigned. So suggesting we do not action this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 22:41:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/160" class=".btn">#160</a>
            </td>
            <td>
                <b>
                    Assign message ID before dispatching message to Kafka in all cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently an ID is only assigned to the message in these cases:
- When using the Webhooks route to input a raw JSON message (`/` or `/hooks`) - before dispatching (to Kafka/sync)
- When explicitly passing a `fly-id`/`kaleido-id` param to the REST API Gateway - before dispatching (to Kafka/sync)
  - Added in #139 
- When the message is received at the Kafka side, and we find no ID inside there

This means in the Kakfa case there is always a message ID assigned at the point of processing.
But in the Sync dispatcher, as used by the FireFly CLI environment, there was no ID being assigned.

We hit an issue with #139 where we found it was leaking through an ID in the REST API Gateway case, that actually came from the gateway ID - that was just fixed in #158.

That fix then in turn exposed the problem of messages ended up with _no ID at all_ and cause the break in the e2e builds for FireFly seen in #159
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 13:17:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/158" class=".btn">#158</a>
            </td>
            <td>
                <b>
                    Honor fly-id for contract deployments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This also prevents bugs where the loaded deployMsg already had an ID and
the ID is reused.

Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 17:47:48 +0000 UTC
    </div>
</div>

