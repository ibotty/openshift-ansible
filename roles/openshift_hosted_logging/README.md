###Required vars:

- openshift_hosted_logging_hostname: kibana.example.com
- openshift_hosted_logging_elasticsearch_cluster_size: 1
- openshift_hosted_logging_master_public_url: https://localhost:8443

###Optional vars:
- openshift_hosted_logging_secret_vars: (defaults to nothing=/dev/null) kibana.crt=/etc/origin/master/ca.crt kibana.key=/etc/origin/master/ca.key ca.crt=/etc/origin/master/ca.crt ca.key=/etc/origin/master/ca.key
- openshift_hosted_logging_fluentd_nodeselector: nodeselector for fluentd
- openshift_hosted_logging_default_nodeselector: default nodeselector
- openshift_hosted_logging_curator_nodeselector: nodeselector for curator
- openshift_hosted_logging_elasticsearch_nodeselector: nodeselector for elasticsearch
- openshift_hosted_logging_kibana_nodeselector: nodeselector for kibana
- openshift_hosted_logging_default_nodeselector: default nodeselector

- openshift_hosted_logging_enable_ops: enable ops cluster. Be sure to set `openshift_hosted_logging_ops_*`.
- openshift_hosted_logging_ops_hostname: hostname for ops cluster
- openshift_hosted_logging_ops_elasticsearch_cluster_size: cluster_size for ops
- openshift_hosted_logging_ops_curator_nodeselector: nodeselector for ops curator
- openshift_hosted_logging_ops_elasticsearch_nodeselector: nodeselector for ops elasticsearch
- openshift_hosted_logging_ops_kibana_nodeselector: nodeselector for ops kibana
