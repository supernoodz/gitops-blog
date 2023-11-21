# Add your pull secret to /root/pullsecret.json

oc create secret docker-registry pull-secret --from-file=.dockerconfigjson=/root/pullsecret.json -n ztp-spoke-01 --dry-run=client -oyaml > 01-unsealed-pull-secret.yaml