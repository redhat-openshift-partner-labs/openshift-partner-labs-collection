# Ansible Collection - opdev.partnerlabs

Documentation for the collection.

### Update the execution environment
```shell
ansible-builder build --container-runtime=podman --tag=quay.io/opdev/openshift-partner-labs-ee:latest --prune-images --verbosity 3
```

### Run the audit
```shell
ansible-navigator run setup.yml --container-engine podman --eei quay.io/opdev/openshift-partner-labs-ee:latest -e @vars.yml --senv K8S_AUTH_KUBECONFIG=/dir/kubeconfig --eev /dir:/dir -m stdout
```

### vars
Documented in vars.yml with default examples included
