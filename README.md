

# build gce instace with a desktop #




openssl pkcs12 -in pkey.pkcs12 -passin pass:notasecret -nodes -nocerts | openssl rsa -out pkey.pem


used to check your yml before you run it
`--syntax-check --list-tasks`

ansible-playbook --syntax-check --list-tasks build_gce.yml


ansible-playbook  build_gce.yml
