# fpf-misc-resources

A repository for publicly available files that are used by other FPF projects.


## Github Actions Workflows

This repo contains a number of reusable workflows that can be integrated in 
other projects. They are located in the `workflows/` directory. These should not
be confused with the `.github/workflows` directory, which contain workflows for 
running this specific repositoriy's CI/CD.

To use one of these workflows in another repository, a snippet like the below can
be added to the Github Actions workflow file, replacing `<workflow>` with the workflow
filename under `workflows/`:

```yaml
jobs:
  myRepoJob:
    uses: freedomofpress/fpf-misc-resources/workflows/<workflow>.yaml
```

For more information on writing and using reusable workflows, see 
[the documentation](https://docs.github.com/en/actions/sharing-automations/reusing-workflows)