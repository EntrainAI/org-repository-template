# .entrain

This organization's Entrain repository: the rules Entrain reviews its pull
requests under.

- `.entrain/rules/` holds the organization's rules, which apply to every pull
  request in its repositories.
- `projects/<key>/.entrain/rules/` holds a project's rules, which apply to the
  pull requests its sessions contribute to in its repositories.

Changing a rule is a pull request here, reviewed under these rules.
`rule-changes` is locked: a change to a rule, an attribute, `.gitattributes` or
`CODEOWNERS` needs a person's approval, the author's included.

Keep the default branch protected, requiring a pull request and the
`entrain/rules` check, so that no direct push changes every repository's rules
unreviewed.
