## 全新安裝

    ```bash
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "action=install" main.yml
    ```

## 重新安裝

    > 先 uninstall 並排除安裝基本套件

    ```bash
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "action=reinstall" main.yml
    ```

## 更新 config

    ```bash
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini main.yml
    ```

## 升級

    ```
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "action=upgrade" main.yml
    ```

## restart service

    ```
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "action=restart" main.yml
    ```