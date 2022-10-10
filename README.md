# ansible-role-sysfs

###### Status: Unstable

(Persistently) set sysfs values

## Example

```yaml
- name: Ensure extra IP addresses
  ansible.builtin.include_role: mangadex.sysfs
  vars:
    sysfs_entries:
      "kernel/mm/transparent_hugepage/enabled": "never"
      "kernel/mm/transparent_hugepage/defrag": "never"
```
