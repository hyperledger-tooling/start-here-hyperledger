---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5854" class=".btn">#5854</a>
            </td>
            <td>
                <b>
                    Bump version to 23.7.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 08:11:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5853" class=".btn">#5853</a>
            </td>
            <td>
                <b>
                    set the beacon root address to the correct value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In EIP-4788 the address of the contract used to store and retrieve the parent beacon block roots has been changed. This PR sets the correct value.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 07:22:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5852" class=".btn">#5852</a>
            </td>
            <td>
                <b>
                    [MINOR] use non-deprecated authenticate methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refs (does not fix) #5851 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 04:11:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5847" class=".btn">#5847</a>
            </td>
            <td>
                <b>
                    Release 23.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Post burn-in release of 23.7.2

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 20:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5844" class=".btn">#5844</a>
            </td>
            <td>
                <b>
                    Range tracing with worldstate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Implement a method to trace a range of blocks and have access to the worldstate before and after the tracing

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 15:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5843" class=".btn">#5843</a>
            </td>
            <td>
                <b>
                    add parent beacon block root to payload id calculation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This fixes a problem where two engine_forkchoiceUpdated RPC calls with the same parameters, except for the parentBeaconBlockRoot, caused besu to produce a block with the wrong block hash.
The beacon root was not used in the calculation of the payload id, which meant that we were not updating the block production after the second call.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 08:10:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5839" class=".btn">#5839</a>
            </td>
            <td>
                <b>
                    [POC] Parallel import during snap sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This is to assess feasibility and potential performance gains

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 13:03:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5838" class=".btn">#5838</a>
            </td>
            <td>
                <b>
                    fix flat db healing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 12:50:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5836" class=".btn">#5836</a>
            </td>
            <td>
                <b>
                    Add world context to transaction tracing API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add world context to the start/end transaction hooks in the tracing API.

## Fixed Issue(s)

fixes: #5835 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 08:00:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5833" class=".btn">#5833</a>
            </td>
            <td>
                <b>
                    ]POC] modify blockchain sync
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 09:45:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5832" class=".btn">#5832</a>
            </td>
            <td>
                <b>
                    Update RocksDB version from 8.0.0 to 8.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

# PR description

Update RocksDB version from 8.0.0 to [8.3.2](https://github.com/facebook/rocksdb/releases/tag/v8.3.2).

<meta charset="utf-8"><b style="font-weight:normal;" id="docs-internal-guid-6dce31b6-7fff-0f91-d7d2-6760648f66be"><h1 dir="ltr" style="line-height:1.38;margin-top:20pt;margin-bottom:6pt;"><span style="font-size:20pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Test setup</span></h1><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Checkpoint Sync with Bonsai on Azure instance Standard_D4s_v5 (4 vCPU, 16 GiB RAM), the starting date of the test is August 31th.</span></p><h1 dir="ltr" style="line-height:1.38;margin-top:20pt;margin-bottom:6pt;"><span style="font-size:20pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Sync time</span></h1><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Sync time is almost the same as there is only one minute difference between RocksDB 8.0.0 and RocksDB 8.3.2</span></p><br /><div dir="ltr" style="margin-left:0pt;" align="left">

RocksDB 8.0.0 | RocksDB 8.3.2
-- | --
21 hours and 21 minutes | 21 hours and 22 minutes

# Block processing time
The block processing time between the two instances is nearly identical. The minor difference is too insignificant to be definitively attributed to this test, and could simply be due to random variation.

</div><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;"><span style="border:none;display:inline-block;overflow:hidden;width:624px;height:283px;"><img src="https://lh3.googleusercontent.com/V016wcdWOl0ZDXC1-63VZOAByNcvXF1Umn4xQ6JRLstf9h4uR1WNLaMoZ1pDSDrfX_xfN2d6yWSjr9lMVAXuOrGwzDDwo3LmUGK_CG4f_zCEXPlAARXo4TigTFF2BV8EbhokGjAkJc3pGTV9zjxKmqg" width="624" height="283" style="margin-left:0px;margin-top:0px;" /></span></span></p><h1 dir="ltr" style="line-height:1.38;margin-top:20pt;margin-bottom:6pt;"><span style="font-size:20pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">System metrics</span></h1><h2 dir="ltr" style="line-height:1.38;margin-top:18pt;margin-bottom:6pt;"><span style="font-size:16pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Memory</span></h2><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Memory usage is quite similar on both nodes</span></p><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;"><span style="border:none;display:inline-block;overflow:hidden;width:624px;height:283px;"><img src="https://lh3.googleusercontent.com/27ALK-LgRX24YIsQP5PAnOvRMBoESinowWX9UyAwXDiTlCJL0_JeKanzn0yiaJMcx9VE85usqiSzKrCZ5trFtR6UQyUad0mmK-ChkFskSW-NP850UBrLO-4l7tc5180Ym9sFoceeG8clixp5yXAsYCI" width="624" height="283" style="margin-left:0px;margin-top:0px;" /></span></span></p><h2 dir="ltr" style="line-height:1.38;margin-top:18pt;margin-bottom:6pt;"><span style="font-size:16pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">CPU&nbsp;</span></h2><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">CPU usage is also very close between RocksDB 8.0.0 and RocksDB 8.3.2</span></p><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;"><span style="border:none;display:inline-block;overflow:hidden;width:624px;height:283px;"><img src="https://lh5.googleusercontent.com/2DNyUYdlPllL8mc57eGR77el4efFr-A0tVaEUqegOl_31TSUXvgY1gQkaZSE-xyw6sJNqduysKdGbLHJr_5KjT3M_AxeYx49uF1jrNsA5A1Ne4kF6zTFAL_SXzQOp_NN3txK7TP77kcW4jtDaKFGTwo" width="624" height="283" style="margin-left:0px;margin-top:0px;" /></span></span></p><h2 dir="ltr" style="line-height:1.38;margin-top:18pt;margin-bottom:6pt;"><span style="font-size:16pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Disk IO</span></h2><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Disk IO activity is pretty similar on both nodes</span></p><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;"><span style="border:none;display:inline-block;overflow:hidden;width:624px;height:283px;"><img src="https://lh4.googleusercontent.com/Bd_0kv-G0fEWKE_uGlyngLo8URsSO4rvt-BZEeX4-PvjKq0pJia-hYHkGFAiXF8MFweJz3NpZoQtfNSckMOWEz5tJPayLhmgAAbINNO5I8jx9TI8_hhJAPcttO8xOPM2XVyh829KSVbM3jUjgEW1r1w" width="624" height="283" style="margin-left:0px;margin-top:0px;" /></span></span></p><br /><h2 dir="ltr" style="line-height:1.38;margin-top:18pt;margin-bottom:6pt;"><span style="font-size:16pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">Network IO</span></h2><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;">There is increased network activity on the node running RocksDB 8.3.2, but this may not be directly related to the RocksDB upgrade. It could simply be associated with peering requests, such as making large requests.</span></p><p dir="ltr" style="line-height:1.38;margin-top:0pt;margin-bottom:0pt;"><span style="font-size:11pt;font-family:Arial,sans-serif;color:#000000;background-color:transparent;font-weight:400;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;white-space:pre;white-space:pre-wrap;"><span style="border:none;display:inline-block;overflow:hidden;width:624px;height:283px;"><img src="https://lh5.googleusercontent.com/6IQkLaxFRmSxDSO4yxAM8yq8fLAxhYbhYbEUpEdu2klunosTCRALUL0P4za0DZ1gJ68RYNYVZCipl0RBMQpUfGiQZY2dfB-ebnaw6LCy7Koc37Fd7Y1Z7hUBAH9Fnp1fD74UbYcYzPwCequbNZgkMtg" width="624" height="283" style="margin-left:0px;margin-top:0px;" /></span></span></p></b><br class="Apple-interchange-newline">

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 09:37:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5831" class=".btn">#5831</a>
            </td>
            <td>
                <b>
                    add versioned hashes and number of blobs to toString()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adding missing information to the toString() method of Transaction
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 06:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5830" class=".btn">#5830</a>
            </td>
            <td>
                <b>
                    Do not create ignorable segments on `revert storage-variables`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The `revert storage-variables` subcommand correctly reverts the storage-variable column family move, but inadvertently creates ignorable column family segments.  This behavior breaks backward compatibility prior to 23.1.0.  

This PR exposes `setIgnorableStorageSegments()` from BesuCommand and calls it from the revert storage-variables subcommand.

Additionally, this PR adds much needed visibility into the column family errors that RocksDB reports by parsing the RocksDBException and translating them into printable strings for more useful/actionable error messages.

example output for unidentified column family:
```
RocksDBException: Unhandled column families: ['Donny'(0x446f6e6e79), 'Walter'(0x57616c746572), 'Maude'(0x4d61756465), 'Dude'(0x44756465)]
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5808 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 23:45:15 +0000 UTC
    </div>
</div>

