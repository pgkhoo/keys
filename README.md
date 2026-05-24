# Encrypted RSA keys for boot-strapping applications

Ensure Apple's command line tools are installed (xcode-select --install to launch the installer).

Install Ansible:

Run the following command to add Python 3 to your $PATH:

export PATH="$HOME/Library/Python/3.9/bin:/opt/homebrew/bin:$PATH"

Clone repo: git clone https://github.com/pgkhoo/keys.git

Install python venv environment: cd keys; python3 -m venv .

Activate venv: . bin/activate

#Upgrade Pip: sudo pip3 install --upgrade pip
#Install Ansible: pip3 install ansible

Upgrade Pip: python3 -m pip install --upgrade pip

Install Ansible: python3 -m pip install ansible

$ ansible-playbook --ask-vault-pass pb_extract_keys.yml

# Tip: decrypt setup script to extract and install RSA keys (pg..06)
openssl aes-256-cbc -d -iter +10000  -in setup.sh.enc

