# Deploy an Ollama server with Docker

This guide will take you through the steps of deploying an Ollama server using Docker.

## What you'll need

To complete this guide, you will need the following:

* A Debian-based system with root access.
* A working QEMU/KVM installation.
* A configured PXE server.
* An internet connection to download the necessary packages and Docker images.

## Procedure

Follow the steps below to deploy an Ollama server with Docker:

1. Add your Debian libvirt host in the Ansible inventory file.

1. Change directory to the Ansible playbook directory:

   ```bash
   user:~$ cd ~/lhammai/ansible
   ```

1. Run the Ansible playbook to deploy the Ollama server:

   ```bash
   user:~/lhammai/ansible$ make all
   ```

   ```{note}
   The playbook will pause two times:
   1. To allow Debian to be installed on the target VM.
   1. To manually install the NVIDIA drivers on the target VM, follow the instructions in the
      [NVIDIA Drivers](nvidia.md) guide.
   You have to press `Enter` to continue the playbook after each pause.
   ```
