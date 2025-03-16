# Ansible Collection - my_own_namespace.yandex_cloud_elk

This Ansible collection provides a simple module to create files with specified content at a given path. It is designed to streamline file management tasks in your playbooks.

## Installation

To install the collection, use the following command:

```
ansible-galaxy collection install my_own_namespace.yandex_cloud_elk
```

## Module: my_own_module

The my_own_module allows you to create a file at a specified path with the provided content.

## Parameters

- `path` (required): The full path where the file will be created.

- `content` (required): The text content to write to the file.

## Example Playbook

```
- name: Create a file with content
  hosts: localhost
  tasks:
    - name: Create a file at /tmp/example.txt
      my_own_namespace.yandex_cloud_elk.my_own_module:
        path: /tmp/example.txt
        content: |
          This is an example file.
          Created using the create_file module.
```

License

This collection is licensed under the MIT License.