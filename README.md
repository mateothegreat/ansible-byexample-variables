```sh
$ ansible-playbook playbook.yml

PLAY [ansible-byexmaples-variables] ************************************************************************************************
TASK [Gathering Facts] *************************************************************************************************************ok: [127.0.0.1]

TASK [Saving a variable to a file] *************************************************************************************************changed: [127.0.0.1]

TASK [debug] ***********************************************************************************************************************ok: [127.0.0.1] => {
    "my_hostsvars_file['127.0.0.1'].ansible_all_ipv4_addresses": [
        "169.254.51.118",
        "10.202.0.2",
        "172.24.198.225",
        "192.168.56.1",
        "169.254.171.142",
        "169.254.219.220",
        "172.17.8.1",
        "192.168.240.1",
        "96.83.34.132",
        "169.254.7.51",
        "96.83.34.131",
        "172.17.181.83"
    ]
}

PLAY RECAP *************************************************************************************************************************127.0.0.1                  : ok=3    changed=1    unreachable=0    failed=0
```