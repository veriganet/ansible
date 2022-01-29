# ansible
ansible

## add nodes

Add nodes to:

`prod/[cloud-region]/inventory.ini`

## install

`ansible-playbook -i ../../prod/aws-eu-west-1/k8s0/inventory.ini -b -v cluster.yml`

## scale up

Run from **vendor/kubespray-2.16.0**:

`ansible-playbook -i ../../prod/aws-eu-west-1/k8s0/inventory.ini scale.yml -b -v --limit "[host1]"`
