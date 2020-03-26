
## Default Variables

### python_global_packages

List of packages to install system-wide

#### Default value

```yaml
python_global_packages: []
```

#### Example usage

```yaml
python_user_gems:
  - requests
  - name: httpie
    verison: 1.0.0
    state: latest
```

### python_install

Install python via homebrew

#### Default value

```yaml
python_install: false
```

### python_pip_executable

Path to python pip executable

#### Default value

```yaml
python_pip_executable: /usr/bin/pip3
```

### python_user

User to run user-specific commands

#### Default value

```yaml
python_user | default(homebrew_user) | default(ansible_user_id)
```

### python_user_packages

List of packages to install for an user

#### Default value

```yaml
python_user_packages: []
```

#### Example usage

```yaml
python_user_gems:
  - requests
  - name: httpie
    verison: 1.0.0
    state: latest
```
## Dependencies

None

## License

Apache-2.0

## Author

Thomas Boerger
