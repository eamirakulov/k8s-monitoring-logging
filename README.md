Tested on Ubuntu 20.04 machine

Run ```ansible-playbook -i inventory/hosts.yml playbooks/main.yml``` to install stack.
```
├── README.md
├── Vagrantfile
├── ansible.cfg
├── inventory
│   └── hosts.yml
├── playbooks
│   └── main.yml
└── roles
    ├── elasticsearch_kibana
    │   ├── defaults
    │   │   └── main.yml
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   ├── install.yml
    │   │   └── main.yml
    │   └── templates
    │       ├── elasticsearch.yml.j2
    │       └── kibana.yml.j2
    ├── fluentbit
    │   ├── defaults
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   └── main.yml
    │   └── templates
    │       └── fluent-bit.conf.j2
    ├── node_exporter
    │   ├── defaults
    │   │   └── main.yml
    │   ├── handlers
    │   │   └── main.yml
    │   ├── tasks
    │   │   ├── config.yml
    │   │   ├── install.yml
    │   │   ├── main.yml
    │   │   └── service.yml
    │   └── templates
    │       └── node_exporter.service.j2
    └── prometheus
        ├── defaults
        │   └── main.yml
        ├── handlers
        │   └── main.yml
        ├── tasks
        │   ├── config.yml
        │   ├── install.yml
        │   ├── main.yml
        │   └── service.yml
        └── templates
            ├── prometheus.service.j2
            └── prometheus.yml.j2
```
