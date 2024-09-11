# Encrypted RSA keys for boot-strapping applications

Ensure Apple's command line tools are installed (xcode-select --install to launch the installer).

$ read -s && echo $REPLY | sha256sum

$ read -s && echo $REPLY | openssl sha256

$ ansible-playbook --ask-vault-pass pb_extract_keys.yml
