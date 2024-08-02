# Encrypted RSA keys for boot-strapping applications

$ read -s && echo $REPLY | sha256sum
$ read -s && echo $REPLY | openssl sha256

$ ansible-playbook --ask-vault-pass pb_extract_keys.yml
