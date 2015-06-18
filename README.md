## Playbooks for deploying Swift

- Host Groups: 
    1. swift_proxy_nodes, 
    2. swift_storage_nodes, 
    3. swift_storage_first_node,

- Roles:
    1. swift-common     --> some parts(apt setup, ntp setup) will be replaced by ansible_system_prepare playbook
    2. swift-proxy
    3. swift-storage-common
    4. swift-storage-first-node
    5. swift-storage-other-nodes
    6. swift-storage-final

- TODO:
    1. Using host_vars to specify detailed specifications of each host for rings
    2. Support multi-region/multi-zone instead of single region and single zone

### NOTICE: NOT TESTED YET.
