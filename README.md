## Call ansible module on the fly
ansible -i hosts localhost -m ping

## Pass inventory and call ansible module on the fly
ansible -i inventories/inventory.txt master -m ping

## Pass inventory and call playbook
ansible-playbook -i inventories/inventory.txt books/pingtest.yaml

##Build on locahost
ansible-playbook build.yaml

## Pass inventory and and key file on the fly
ansible-playbook -i 'test.mukeshgupta.info,' remote.yaml --key-file key.pem

