# sandbox-environments
## Summary
Repo holding all environments in the DIPS sandbox

For each branch created in this repo an environment will be spun up in the .api.dips.no domain.
URL to the spun up environment is [branch-name].api.dips.no.

The configuration from this branch is used and can be changed according to your needs. You can also make changes to the yaml file specifying all the nodes in Kubernetes cluster for the environment. All nodes are spun up in a namespace.

Illegal characters in the branch-name are replaced by dashes (-).

## Files

The default files will create a sandbox environment out of the box. Feel free to change the files inside your branch to customize your sandbox.

* manifest.yaml  
This is the Kubernetes manifest describing all the nodes in the environment cluster making up the sandbox environment.

* configuraton.json
The dips-configuration-service reads this json and all values are available to consumers of this service.

TEST: 2021.04.15 Trigging push to Git repo and WebHook
TEST: 2021.04.16 Trigging yet another push - and again and again
