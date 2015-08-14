

# build gce instace with a desktop #


# service account information  #

##  skc-base-project ##

    Service account
    Client ID
    46088636398-s6v0nurnmfp89c96r9l26r334695og17.apps.googleusercontent.com
    Email address
    46088636398-s6v0nurnmfp89c96r9l26r334695og17@developer.gserviceaccount.com
    Certificate fingerprints
    
        b95c375cba17b2118738ed3159112d8259eacd10


<http://docs.ansible.com/ansible/guide_gce.html>



openssl pkcs12 -in pkey.pkcs12 -passin pass:notasecret -nodes -nocerts | openssl rsa -out pkey.pem

openssl pkcs12 -in skc-base-project-2302fab56bbc.p12 -passin pass:notasecret -nodes -nocerts | openssl rsa -out pkey.pem

openssl pkcs12 -in skc-gce-ansible-01-b08aa1c65854.p12 -passin pass:notasecret -nodes -nocerts | openssl rsa -out pkey.pem

used to check your yml before you run it
`--syntax-check --list-tasks`

ansible-playbook --syntax-check --list-tasks build_gce.yml


ansible-playbook  build_gce.yml
