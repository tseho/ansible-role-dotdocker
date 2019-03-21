# ansible-role-dotdocker

## Install
```
ansible-galaxy install tseho.dotdocker
```

## Options

List of optional variables:
```
dotdocker_autostart: yes                # If dotdocker run docker-compose up -d
dotdocker_docker_sync_enabled: yes      # If docker-sync should be configured on OSX

dotdocker_user_id: ~                    # Id of the current user, for files permissions
dotdocker_project_path: ~               # Project root directory, "../" by default
dotdocker_path: ~                       # dotdocker real path, "../.docker" by default
dotdocker_project_name: ~               # Project name, use directory name by default
dotdocker_virtual_host: ~               # {{ dotdocker_project_name }}.localhost by default
dotdocker_compose_override_template: ~  # "../.docker/.templates/docker-compose.override.<OS>.yml.j2"
dotdocker_docker_sync_template: ~       # "../.docker/.templates/docker-sync.yml.j2"
dotdocker_env: {}                       # List of environment variables to set in ".docker/.env"
```
Unspecified variables are defined on runtime by the role.
