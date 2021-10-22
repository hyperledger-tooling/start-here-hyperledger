---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/229" class=".btn">#229</a>
            </td>
            <td>
                <b>
                    Update rust docs for sabre protocols
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 21:26:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    Add release notes for 0.3.12
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
        Created At 2021-10-21 20:18:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    sabre protocol doc typo fixes
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
        Created At 2021-10-21 19:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    Fix typo in doc comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 19:25:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/225" class=".btn">#225</a>
            </td>
            <td>
                <b>
                    Backport 0-3: Multi-threaded bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backports PR #222 into 0-3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 19:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/224" class=".btn">#224</a>
            </td>
            <td>
                <b>
                    Fix typo in rustdoc for SabreContext.add_receipt_data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 17:55:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/223" class=".btn">#223</a>
            </td>
            <td>
                <b>
                    Backport 0-3: Limit recursion to same tree ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Back-port of #221 to 0-3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 16:38:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/222" class=".btn">#222</a>
            </td>
            <td>
                <b>
                    Multi-threaded bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a test for multi-threaded reads using merkle state implementations.  This test identified several issues with the SqlMerkleState sqlite and postgres implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 01:26:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/221" class=".btn">#221</a>
            </td>
            <td>
                <b>
                    Limit recursion to same tree ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change limits the SQL recursion to the same tree_id.  This prevents an issue where the existence of multiple trees with duplicate structure creates an infinite loop in SQLite.

The same change has been applied to the recursive queries in Postgres.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 15:27:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/220" class=".btn">#220</a>
            </td>
            <td>
                <b>
                    Update workload to check batch result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update `TransactionWorkload`'s `next_transaction` and `BatchWorkload`'s `next_batch` to return an optional `ExpectedBatchResult`. ExpectedBatchResult is an enum with variants `Valid` and Invalid` to indicate the expected outcome of a batch after it has been submitted to a target.
- Update the `next_transaction` and `next_batch` methods in the command implementation of `TransactionWorkload`  and `BatchWorkload` to return an `ExpectedBatchResult` based on the type of transaction being submitted. The `next_transaction` and `next_batch` methods in the smallbank implementation were updated to return None for now as it is not possible to determine the expected result of an amalgamate transaction.
- Add an arg `get_batch_status` to `add_workload` and pass this arg's value to the `WorkerBuilder` `get_batch_status` method. This arg is a boolean value that determines if the worker will check the status of batches after they are submitted to determine if the expected outcome was achieved. This value is set to true when starting a command workload and false when starting a smallbank workload because smallbank does not report the expected outcome of transactions as mentioned above.
- Update the `submit_batch` method to deserialize the REST API response to get the batch status link and return it. The returned link is stored as the key in a HashMap mapped to the target the batch was submitted to and the expected batch result.
- Add a method `check_batch_status` that takes the HashMap containing the batch status links and expected batch results and loops through the links checking if the batch status matches what was expected. If the status link returns the expected result the link is removed from the list so that it will not be checked again. If the status is pending the link will be left in the list so that it can be checked again on the next iteration. `check_batch_status` is called at the end of the loop in the `WorkerBuilder` `build` method if `get_batch_status` is true.

If a command workload is being run and the batch result doesn't match the expected batch result that was set the workload will stop and report an error like the following:
`Unable to submit batch: Expected valid result, received invalid [InvalidTransaction { transaction_id: "5b933e612a09382b2054b7cb53a8bb2f6c1abc3fcb797a8dff08ac6233317fdf279c60d733af0169e3f0bc85a4de5676c07665ce70bfea824702775c0dc8909e", error_message: "Wasm contract returned invalid transaction: command, 1.0", error_data: [] }]`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 20:32:28 +0000 UTC
    </div>
</div>

