#Install and Setup Ansible 

# Install boto3
```sh 
pip install boto3
```

# Install aws collection
```sh 
ansible-galaxy collection install amazon.aws
```

# Setup vault
```sh
openssl rand -base64 2048 > vault.pass
```

# Create the vault for  the AWS Credentials
```sh 
openssl-vault create group_vars/all/pass.yml --vault-password-file vault.pass
``` 
