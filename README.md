Install docker-compose and Grafana/Prometheus/AlertManager/Loki + node-exporter/cadvisor

Only Ubuntu Ubuntu 20.04/LTS

1. Set hosts and users with root permissions in inventory/hosts.ini
2. ansible-playbook -i inventory/hosts.ini fullinstall.yaml --ask-vault-pass 

docker-compose.yaml - install docker and docker-compose 

observability.yaml - install Grafana/Prometheus/AlertManager/Loki + node-exporter/cadvisor

fullinstall.yaml - include docker-compose.yaml and observability.yaml
