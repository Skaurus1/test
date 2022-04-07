Install docker-compose and Grafana/Prometheus/AlertManager/Loki + node-exporter/cadvisor

Only Ubuntu 20.04/LTS

1. Set hosts and users with root permissions in inventory/hosts.ini
2. Specify email for notification in inventory/group_vars/prod/vars.yaml
3. ansible-playbook -i inventory/hosts.ini fullinstall.yaml --ask-vault-pass 

docker-compose.yaml - install docker and docker-compose 

observability.yaml - install Grafana/Prometheus/AlertManager/Loki + node-exporter/cadvisor

fullinstall.yaml - include docker-compose.yaml and observability.yaml

grafana listens on port 3000
