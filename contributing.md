# Contribution guidelines

## Rules

- Add one tool in each pull request.
- Use this format: `- [Name](https://link) - Description.`
- Write the description as one short sentence. End it with a period.
- Put the tool under the correct sub-heading, in A to Z order.
- If no sub-heading fits, add a new `###` sub-heading.
- If no section fits, add a new `##` section. Also add it to the Contents list.
- Link to the official website of the tool.
- Make sure that the tool is not already in the list.

## Steps on the GitHub website

1. Find an issue with the label `good first issue`, or choose your own tool.
2. If you take an issue, write a comment on it, so that other students know.
3. Click **Fork** at the top of this repository.
4. In your fork, open `README.md` and click the pencil icon.
5. Add your line.
6. Click **Commit changes**. Write a short message, for example `Add Audacity`.
7. Click **Contribute**, then **Open pull request**.
8. If your pull request solves an issue, write `Closes #` and the issue number in the description.
9. Wait for the checks. If a check is red, open its details, fix your line, and commit again.

## Steps in the terminal

```sh
gh repo fork HEAD-MasterMediaDesign/resource-awesome-media-design --clone
cd resource-awesome-media-design
git switch -c add-audacity
# edit README.md
git commit -am "Add Audacity"
git push -u origin add-audacity
gh pr create --fill
```
