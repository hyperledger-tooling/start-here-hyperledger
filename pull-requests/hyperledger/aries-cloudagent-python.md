---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2705" class=".btn">#2705</a>
            </td>
            <td>
                <b>
                    feat: inject profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the Profile to the injection context. This enables creating a `ClassProvider` for a class that takes a profile in its init method:

```python
class ExamplePluggable:
    def __init__(self, profile: Profile):
        self.profile = profile
    def do_something(self):
        self.profile.notify("some:event", {"with": "data"})

async def setup(context: InjectionContext):
    context.injector.bind_provider(
        ExamplePluggable,
        ClassProvider(ExamplePluggable, ClassProvider.Inject(Profile))
    )

# ... Somewhere else ...
plugged_in = profile.inject(ExamplePluggable)
plugged_in.do_something()
```

It's a common pattern to create a class with a profile instance. This will make it easier to turn some of these components into pluggable components. For example, the `VcLdpManager`. At the moment, it's created directly where it's needed:

```python
manager = VcLdpManager(self.profile)
# do something with manager
```

With this change, I can create an (override-able) class provider for VcLdpManager, which changes the above into:

```python
manager = self.profile.inject(VcLdpManager)
# do something with manager
```

The only way this could be done previously was by binding providers in the Profile init method itself. This made it more difficult to make more components pluggable.

Side note: it's critical that the profile instance be injected as a weak reference or it will never be "finalized" (garbage collected) in multitenant contexts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 14:56:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2704" class=".btn">#2704</a>
            </td>
            <td>
                <b>
                    fix: minor type hint corrections for VcLdpManager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are some really minor fixes just to make type checking happy and to clarify the use of some values in the VcLdpManager.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 13:18:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2700" class=".btn">#2700</a>
            </td>
            <td>
                <b>
                    Update legacy bcgovimages references.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves: #2118 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 19:48:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2699" class=".btn">#2699</a>
            </td>
            <td>
                <b>
                    Remove tiny-vim from being added to the container image to reduce reported vulnerabilities from scanning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 18:42:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2698" class=".btn">#2698</a>
            </td>
            <td>
                <b>
                    fix: update constants in TransactionRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves: #1650
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 22:28:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2696" class=".btn">#2696</a>
            </td>
            <td>
                <b>
                    Feature/emit did peer 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Open for comments on how to update the long form with the short form. The resolver handles its own mapping, however i'm storing a duplicate DIDInfo, one where the did is long form and another where it's short form (for the same verkey). 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 00:03:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2694" class=".btn">#2694</a>
            </td>
            <td>
                <b>
                    fix: save multi_use to the DB for OOB invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was reported by a collegue that when using Out-of-band invitations with the connections handshake protocol, along with a public DID and connection re-use enabled, ACA-Py was only able to handle a single invitations. As if Connection Re-use wasn't working or the multi_use flag was ignored.

Turns out, we flat out weren't saving the multi_use flag to the database which is a big problem if you want to re-use the invitation. When DID-Exchanged is used, since DID-Exchange allows for a connection-less exchange of information. We only say the behaviour of the OOB Invitation getting deleted if we ran through the receive_reuse_message() method in the manager, which deletes the record if it's not set for multi_use.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 19:08:12 +0000 UTC
    </div>
</div>

