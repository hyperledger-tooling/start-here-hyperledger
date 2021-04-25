---
layout: default
title: {{.Repository.Name}}
parent: {{.Organization.Name}}
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/{{.Organization.Github}}/{{.Repository.Name}}
---

# {{.Repository.Name}}

You can clone this repo on <span class="fs-3">[GitHub]({{.Repository.Link}}){: .btn .mr-4 }</span>

{{range .PRs}}
<div>
    <table>
        <tr>
            <td>
                PR [#{{.Number}}]({{.URL}})
            </td>
            <td>
                <b>
                    {{.Title}}
                </b>
            </td>
        </tr>
        <tr>
            <td>
                {{range .Labels}}{{.Name}}{: .label-grey }{{end}}
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
