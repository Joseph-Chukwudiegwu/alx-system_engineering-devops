# `SSH`
SSH (Secure Shell) is a secure network protocol used for remote access and management of network devices, servers, and computers over an unsecured network, such as the Internet
# Resources
# A Simple SSH Illustration
![](https://assets.website-files.com/5ff66329429d880392f6cba2/61c1b963247368113bbeef17_Secure%20Shell%20work.png)


# Learning Objectives
## General
- What is a server
- Where servers usually live
- What is SSH
- How to create an SSH RSA key pair
- How to connect to a remote host using an SSH RSA key pair
- The advantage of using #!/usr/bin/env bash instead of /bin/bash

- Connecting to and working
with servers using the SSH protocol.

## Tasks :page_with_curl:

* **0. Use a private key**
  * [0-use_a_private_key](./0-use_a_private_key): Bash script that uses `ssh` to connect to my
server.

* **1. Create an SSH key pair**
  * [1-create_ssh_key_pair](./1-create_ssh_key_pair): Bash script that creates an RSA key pair.

* **2. Client configuration file**
  * [2-ssh_config](./2-ssh_config): SSH configuration file configured to use the private key
`~/.ssh/school` and to refuse authentication using a password.

* **3. Let me in!
  * Now that you have successfully connected to your server, we would also like to join the party.

  * Add the SSH public key below to your server so that we can connect using the ubuntu user.

<table class="table table-striped">
  <thead>
    <tr>
      <th>Name</th>
      <th>Username</th>
      <th>IP</th>
      <th>State</th>
      <th></th>
    </tr>
  </thead>

  <tbody>
      <tr>
        <td>59637-web-01</td>
        <td><code>ubuntu</code></td>
        <td><code>52.23.212.37</code></td>
        <td>running</td>
        <td>
          <div class="btn-group">
            <button type="button" class="btn btn-sm btn-default dropdown-toggle" data-toggle="dropdown">
              Actions
              <span class="caret"></span>
              <span class="sr-only">Toggle Dropdown</span>
            </button>
            <ul class="dropdown-menu dropdown-menu-right">
                <li><a data-confirm="Are you sure to reboot 59637-web-01?" href="/servers/9390/soft_reboot">Soft reboot</a></li>
                  <li><a data-confirm="Are you sure to hard reboot 59637-web-01?" href="/servers/9390/hard_reboot">Hard reboot</a></li>

              <li role="separator" class="divider"></li>

                <li>
                  <a data-confirm="Are you sure you'd like a new server?
- This server will be destroyed
- Did you update your public SSH key in your user profile yet?

This action can take time...
Please, be patient..." href="/servers/9390/ask_new">
                    Ask a new server
</a>                </li>
            </ul>
          </div>
        </td>
      </tr>
    
  </tbody>
</table>
