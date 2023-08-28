---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4405" class=".btn">#4405</a>
            </td>
            <td>
                <b>
                    Update install scripts for v2.5.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix
- Documentation update

#### Description

Update install script and bootstrap script for v2.5.4.

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 05:20:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4402" class=".btn">#4402</a>
            </td>
            <td>
                <b>
                    CFT Block Puller: reset total sleep 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Bug fix

#### Description

In internal/pkg/peer/blocksprovider/deliverer.go:150

Local variable `totalDuration` measures the total sleep during retries. If it exceeds `reconnectTotalTimeThreshold` the Deliverer may exit if `MaxRetryDurationExceededHandler` returns true. 

However, it does not reset on success (block reception), so `DeliverBlocks()` may exit eventually if the cumulative sleep time is large, but no consecutive reconnect failure sequence exceeds the threshold for stopping retries.

The solution is to reset `totalDuration` together when we reset `failureCounter`.


#### Related issues

Issue: #4394 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-27 11:56:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4398" class=".btn">#4398</a>
            </td>
            <td>
                <b>
                    up smartbft library
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
        Created At 2023-08-25 05:06:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4397" class=".btn">#4397</a>
            </td>
            <td>
                <b>
                    Improve add_orderer.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates add_orderer.md to improve it from the user's perspective.

#### Type of change
- Documentation update

#### Description
I'm trying out the BFT samples in fabric-samples recently.
As part of this process, I also tried to add an orderer following the instructions in the doc added by https://github.com/hyperledger/fabric/pull/4390.

I've identified some areas from a user's perspective that might benefit from further improvements.
This PR updates add_orderer.md for the above improvements.

#### Other possible improvements, or points that were not clear after trying the procedure

- I interpreted that [such a file path description](https://github.com/hyperledger/fabric/blob/17b77cf1d8750263df89316cd0c888f18b872022/docs/source/create_channel/add_orderer.md?plain=1#L185) in Add the fifth orderer to the config should actually be filled in with the result of base64 encoding of the certificate in the file, but some readers may overlook it.
  - It may be less misleading to explicitly state in a snippet, such as `<The result of base64 encoding of the contents in ...>`.

- It might be more user-friendly if the command snippets for entering `cli` container and copying between cli and local were also illustrated in the doc.

#### Related issues
https://github.com/hyperledger/fabric/issues/4332

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 03:56:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4396" class=".btn">#4396</a>
            </td>
            <td>
                <b>
                    connecting smartbft metrics
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
        Created At 2023-08-24 19:25:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4395" class=".btn">#4395</a>
            </td>
            <td>
                <b>
                    Do not send channel name as part of each message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the new communication infrastructure implementation, as per the RFC [0], the channel name for the entire lifetime of the gRPC stream, is determined at the time of establishing and authenticating the gRPC stream, and therefore there is no need to send the channel name in each message.

[0] https://hyperledger.github.io/fabric-rfcs/text/orderer-v3.html#orderer-to-orderer-authentication-and-communication

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-24 13:21:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4393" class=".btn">#4393</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: seek content type header+sig to send full config bl…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Improvement (improvement to code)
- Test update


#### Description

As described in issue #4354


#### Related issues

issue #4354 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 15:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4392" class=".btn">#4392</a>
            </td>
            <td>
                <b>
                    delete ioutil pkg and redundant type casting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ioutil.Discard -> os.Discard
ioutil.NopCloser -> io.NopCloser
delete redundant type casting
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 08:00:46 +0000 UTC
    </div>
</div>

