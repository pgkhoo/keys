# Encrypted RSA keys for boot-strapping applications

Ensure Apple's command line tools are installed (xcode-select --install to launch the installer).

Install Ansible:

Run the following command to add Python 3 to your $PATH: export PATH="$HOME/Library/Python/3.9/bin:/opt/homebrew/bin:$PATH"
Upgrade Pip: sudo pip3 install --upgrade pip
Install Ansible: pip3 install ansible
Ensure that homebrew is installed

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

$ read -s && echo $REPLY | sha256sum

$ read -s && echo $REPLY | openssl sha256

$ ansible-playbook --ask-vault-pass pb_extract_keys.yml
