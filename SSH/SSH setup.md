```
network:
  version: 2
  ethernets:
    eth0:
      dhcp4: no
      addresses:
        - (Shell/FTP ip)
      gateway4: (competition router ip)
      nameservers:
        addresses:
          - 8.8.8.8
          - 8.8.4.4
```
![[{2981CE34-120A-4A89-AF71-61F34F7ACA4A}.png]]

```
#!/bin/bash

# Array of users
users=(
  user
  user
  user (name all users)
  user
  user
)

# Loop through each user
for user in "${users[@]}"; do

  # Create the user if they don't exist(add only if user doesnt exist)
  if ! id -u "$user" >/dev/null 2>&1; then
    sudo useradd -m "$user"
  fi

  # Create .ssh directory
  sudo mkdir -p /home/"$user"/.ssh

  # Copy the public key to authorized_keys
  sudo cp /home/blueteam/"$user".pub /home/"$user"/.ssh/authorized_keys

  # Set the correct permissions
  sudo chmod 700 /home/"$user"/.ssh
  sudo chmod 600 /home/"$user"/.ssh/authorized_keys
  sudo chown -R "$user":"$user" /home/"$user"/.ssh
done

echo "SSH keys have been set up for all users."
```

*To use this script*:

1. Save it to a file, for example, `setup_ssh_keys.sh`.
2. Make the script executable:
    
    ```
    chmod +x setup_ssh_keys.sh
    ```
    
3. Run the script:
    
    ```
    sudo ./setup_ssh_keys.sh
    ```
