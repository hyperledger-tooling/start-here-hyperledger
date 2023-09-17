---
layout: default
title: sawtooth-core
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-core
---

# sawtooth-core <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-core){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2458" class=".btn">#2458</a>
            </td>
            <td>
                <b>
                    fix(commit_store): fix bug in `get_batch_by_transaction`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `sawtooth_validator::journal::commit_store::CommitStore::get_batch_by_transaction` contains a bug where the method will return the first batch that does **not** contain the provided `transaction_id` without any error. 

The equivalent Python method calls the Rust method via FFI

```python
# validator/sawtooth_validator/journal/block_store.py

def get_batch_by_transaction(self, transaction_id):
        """
        Check to see if the requested transaction_id is in the current chain.
        If so, find the batch that has the transaction referenced by the
        transaction_id and return the batch. This is done by finding the block
        and searching for the batch.

        :param transaction_id (string): The id of the transaction that is being
            requested.
        :return:
        The batch that has the transaction.
        """
        payload = self._get_data_by_id(
            transaction_id, 'commit_store_get_batch_by_transaction')

        batch = Batch()
        batch.ParseFromString(payload)

        return batch
```

Here's `commit_store_get_batch_by_transaction`

```rust
//! validator/src/journal/commit_store_ffi.rs

#[no_mangle]
pub unsafe extern "C" fn commit_store_get_batch_by_transaction(
    commit_store: *mut c_void,
    transaction_id: *const c_char,
    batch_ptr: *mut *const u8,
    batch_len: *mut usize,
    batch_cap: *mut usize,
) -> ErrorCode {
    check_null!(commit_store, transaction_id);

    match deref_cstr(transaction_id) {
        Ok(transaction_id) => {
            match (*(commit_store as *mut CommitStore)).get_batch_by_transaction(transaction_id) {
                Ok(batch) => return_batch(batch, batch_ptr, batch_len, batch_cap),
                Err(err) => map_database_error(err),
            }
        }
        Err(err) => err,
    }
}
```

---
Signed-off-by: Joseph Livesey [jlivesey@gmail.com](mailto:jlivesey@gmail.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 14:45:12 +0000 UTC
    </div>
</div>

