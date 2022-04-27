# ssh_full_mesh
 Build full mesh SSH authorized keys between listed hosts for root or provided user

    ansible-playbook -i hosts ssh_keys_fullmesh.yml -u root --ask-pass
    
 User can be passed to ansible script via `hosts` file as variable: *ssh_key_user*.
 When this variable is not defined, default full mesh SSH keys will be generated for root user.
 As an alternative for setting up variable in the `hosts` file, there is possibility to set this
 in a command line extension: `-e ssh_key_user=<user>`
