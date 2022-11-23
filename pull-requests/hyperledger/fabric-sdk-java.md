---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Change executor service defaults (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Set the default core and maximum thread pool size to Runtime.getRuntime().availableProcessors().
- Use a fixed thread pool using the larger of core or maximum thread pool, and an unbounded queue to prevent failures submitting work when all threads are in use.
- Make HFClient.getExecutorService() public.

The default (effectively) unlimited thread pool size could cause so many threads to be created under high event load that system failures could occur.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 13:40:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/241" class=".btn">#241</a>
            </td>
            <td>
                <b>
                    Change executor service defaults
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Set the default core and maximum thread pool size to Runtime.getRuntime().availableProcessors().
- Use a fixed thread pool using the larger of core or maximum thread pool, and an unbounded queue to prevent failures submitting work when all threads are in use.
- Make HFClient.getExecutorService() public.

The default (effectively) unlimited thread pool size could cause so many threads to be created under high event load that system failures could occur.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 13:39:10 +0000 UTC
    </div>
</div>

