# SSH

This folder contains the SSH project files.

## Task 0
Use the private key `~/.ssh/school` to connect to your server as `ubuntu`.

Pass the server IP as the first argument to `0-use_a_private_key`, or replace `YOUR_SERVER_IP` in the script once the facilitator gives you the server details.

## Task 1
Generate a 4096-bit RSA key pair named `school` with the passphrase `betty`.

## Task 2
Use the SSH client config in `2-ssh_config` so SSH uses `~/.ssh/school` and refuses password authentication.

## Task 3
Add the given public key to the server's `~/.ssh/authorized_keys` file for the `ubuntu` user.

Run the following on the server once you are connected:

```bash
mkdir -p ~/.ssh
chmod 700 ~/.ssh
echo 'ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDNdtrNGtTXe5Tp1EJQop8mOSAuRGLjJ6DW4PqX4wId/Kawz35ESampIqHSOTJmbQ8UlxdJuk0gAXKk3Ncle4safGYqM/VeDK3LN5iAJxf4kcaxNtS3eVxWBE5iF3FbIjOqwxw5Lf5sRa5yXxA8HfWidhbIG5TqKL922hPgsCGABIrXRlfZYeC0FEuPWdr6smOElSVvIXthRWp9cr685KdCI+COxlj1RdVsvIo+zunmLACF9PYdjB2s96Fn0ocD3c5SGLvDOFCyvDojSAOyE70ebIElnskKsDTGwfT4P6jh9OBzTyQEIS2jOaE5RQq4IB4DsMhvbjDSQrP0MdCLgwkN' >> ~/.ssh/authorized_keys
chmod 600 ~/.ssh/authorized_keys
```
