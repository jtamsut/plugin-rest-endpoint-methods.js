---
name: Delete a repository variable
example: octokit.rest.actions.deleteRepoVariable({ owner, repo, name })
route: DELETE /repos/{owner}/{repo}/actions/variables/{name}
scope: actions
type: API method
---

# Delete a repository variable

Deletes a repository variable using the variable name.
You must authenticate using an access token with the `repo` scope to use this endpoint.
GitHub Apps must have the `actions_variables:write` repository permission to use this endpoint.

```js
octokit.rest.actions.deleteRepoVariable({
  owner,
  repo,
  name,
});
```

## Parameters

<table>
  <thead>
    <tr>
      <th>name</th>
      <th>required</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>owner</td><td>yes</td><td>

The account owner of the repository. The name is not case sensitive.

</td></tr>
<tr><td>repo</td><td>yes</td><td>

The name of the repository. The name is not case sensitive.

</td></tr>
<tr><td>name</td><td>yes</td><td>

The name of the variable.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/actions/variables#delete-a-repository-variable).
