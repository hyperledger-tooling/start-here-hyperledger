---
layout: default
title: learning-tokens
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/learning-tokens
---

# learning-tokens <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/learning-tokens){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Issue#27 / Draft 1 : Email template for Invitation to Learners by Instructors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## About 
- A Draft Email Template for Invitation to Courses by Instructors to their learners. 

## Future Scope
- Can be extended to include all notifications, updates, reminders, invitations from Institutions to Instructors. 
- API integration using Zoho / Resend / MailChimp, etc. 

## Extensive Documentation
- Can API Integration be done purely using React? No. I discuss [here](https://github.com/NeoZ666/react-email-starter/blob/main/readme.md#why-you-cant-send-emails-purely-using-react-) why is that the case.
- [Standalone Repository](https://github.com/NeoZ666/react-email-starter) for exploring, extending the template.
- Live Demo of Email [here](https://codesandbox.io/p/github/NeoZ666/react-email-starter/main?import=true&layout=%257B%2522sidebarPanel%2522%253A%2522GIT%2522%252C%2522rootPanelGroup%2522%253A%257B%2522direction%2522%253A%2522horizontal%2522%252C%2522contentType%2522%253A%2522UNKNOWN%2522%252C%2522type%2522%253A%2522PANEL_GROUP%2522%252C%2522id%2522%253A%2522ROOT_LAYOUT%2522%252C%2522panels%2522%253A%255B%257B%2522type%2522%253A%2522PANEL_GROUP%2522%252C%2522contentType%2522%253A%2522UNKNOWN%2522%252C%2522direction%2522%253A%2522vertical%2522%252C%2522id%2522%253A%2522clvwvwl6k00062a6bguh273nk%2522%252C%2522sizes%2522%253A%255Bnull%252Cnull%255D%252C%2522panels%2522%253A%255B%257B%2522type%2522%253A%2522PANEL_GROUP%2522%252C%2522contentType%2522%253A%2522EDITOR%2522%252C%2522direction%2522%253A%2522horizontal%2522%252C%2522id%2522%253A%2522EDITOR%2522%252C%2522panels%2522%253A%255B%257B%2522type%2522%253A%2522PANEL%2522%252C%2522contentType%2522%253A%2522EDITOR%2522%252C%2522id%2522%253A%2522clvwvwl6k00022a6bpjmf6v7o%2522%257D%255D%257D%252C%257B%2522type%2522%253A%2522PANEL_GROUP%2522%252C%2522contentType%2522%253A%2522SHELLS%2522%252C%2522direction%2522%253A%2522horizontal%2522%252C%2522id%2522%253A%2522SHELLS%2522%252C%2522panels%2522%253A%255B%257B%2522type%2522%253A%2522PANEL%2522%252C%2522contentType%2522%253A%2522SHELLS%2522%252C%2522id%2522%253A%2522clvwvwl6k00042a6bxwzvvk4d%2522%257D%255D%252C%2522sizes%2522%253A%255B100%255D%257D%255D%257D%252C%257B%2522type%2522%253A%2522PANEL_GROUP%2522%252C%2522contentType%2522%253A%2522DEVTOOLS%2522%252C%2522direction%2522%253A%2522vertical%2522%252C%2522id%2522%253A%2522DEVTOOLS%2522%252C%2522panels%2522%253A%255B%257B%2522type%2522%253A%2522PANEL%2522%252C%2522contentType%2522%253A%2522DEVTOOLS%2522%252C%2522id%2522%253A%2522clvwvwl6k00052a6brs9altel%2522%257D%255D%252C%2522sizes%2522%253A%255B100%255D%257D%255D%252C%2522sizes%2522%253A%255B50%252C50%255D%257D%252C%2522tabbedPanels%2522%253A%257B%2522clvwvwl6k00022a6bpjmf6v7o%2522%253A%257B%2522id%2522%253A%2522clvwvwl6k00022a6bpjmf6v7o%2522%252C%2522activeTabId%2522%253A%2522clvwx9bo200h82a6bn6yb76ov%2522%252C%2522tabs%2522%253A%255B%257B%2522id%2522%253A%2522clvwvwl6j00012a6bngu23cxq%2522%252C%2522mode%2522%253A%2522permanent%2522%252C%2522type%2522%253A%2522FILE%2522%252C%2522filepath%2522%253A%2522%252F.gitignore%2522%252C%2522state%2522%253A%2522IDLE%2522%257D%252C%257B%2522type%2522%253A%2522FILE%2522%252C%2522filepath%2522%253A%2522%252F.codesandbox%252Ftasks.json%2522%252C%2522id%2522%253A%2522clvwx9bo200h82a6bn6yb76ov%2522%252C%2522mode%2522%253A%2522permanent%2522%257D%255D%257D%252C%2522clvwvwl6k00052a6brs9altel%2522%253A%257B%2522id%2522%253A%2522clvwvwl6k00052a6brs9altel%2522%252C%2522tabs%2522%253A%255B%257B%2522type%2522%253A%2522TASK_PORT%2522%252C%2522taskId%2522%253A%2522dev%2522%252C%2522port%2522%253A3000%252C%2522id%2522%253A%2522clvwx979r00g42a6bj1lkn60x%2522%252C%2522mode%2522%253A%2522permanent%2522%252C%2522path%2522%253A%2522%252Fpreview%252Findex%2522%257D%255D%252C%2522activeTabId%2522%253A%2522clvwx979r00g42a6bj1lkn60x%2522%257D%252C%2522clvwvwl6k00042a6bxwzvvk4d%2522%253A%257B%2522id%2522%253A%2522clvwvwl6k00042a6bxwzvvk4d%2522%252C%2522tabs%2522%253A%255B%257B%2522id%2522%253A%2522clvwvwl6k00032a6byrh7qjqw%2522%252C%2522mode%2522%253A%2522permanent%2522%252C%2522type%2522%253A%2522TERMINAL%2522%252C%2522shellId%2522%253A%2522clvwvzvpm0011dieocbr5ew9g%2522%257D%252C%257B%2522type%2522%253A%2522TASK_LOG%2522%252C%2522taskId%2522%253A%2522dev%2522%252C%2522id%2522%253A%2522clvwvxyqv00cf2a6b68dgodg4%2522%252C%2522mode%2522%253A%2522permanent%2522%257D%255D%252C%2522activeTabId%2522%253A%2522clvwvxyqv00cf2a6b68dgodg4%2522%257D%257D%252C%2522showDevtools%2522%253Atrue%252C%2522showShells%2522%253Atrue%252C%2522showSidebar%2522%253Atrue%252C%2522sidebarPanelSize%2522%253A15%257D)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 21:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/learning-tokens/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Issue#25 : Frontend for Modal Component for Sending Invite Mails to Learners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Made frontend-only changes to the react components with path `src/learning-token-dashboard/src/pages/instructor/index.tsx` . Added Emailing functionality to multiple Emails. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-07 19:23:56 +0000 UTC
    </div>
</div>

