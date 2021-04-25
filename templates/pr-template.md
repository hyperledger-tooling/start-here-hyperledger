---
layout: default
title: {{.Repository.Name}}
parent: {{.Organization.Name}}
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/{{.Organization.Github}}/{{.Repository.Name}}
---

# {{.Repository.Name}} <span class="fs-3 right-align">[GitHub]({{.Repository.Link}}){: .btn .mr-4 }</span>

{{range .PRs}}
<div>
    <table>
        <tr>
            <td>
                PR <a href="{{.HTMLURL}}" class=".btn">#{{.Number}}</a>
            </td>
            <td>
                <b>
                    {{.Title}}
                </b>
            </td>
        </tr>
        <tr>
            <td>
                {{range .Labels}}<span class="chip">{{.Name}}</span>{{end}}
            </td>
            <td>
                {{.Body}}
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At {{.CreatedAt}}
    </div>
</div>
{{end}}
