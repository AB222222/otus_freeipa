# otus_freeipa

Сервер развёрнут вручную (не было задачи ставить его через Ansible). 

Логи и пароль админа: admin : Password1

Клиент при развёртывании регистрируется на сервере FreeIPA и может получить тикет:

```
me@me-HP-260-G3-DM:~/otus-linux/DZ_FreeIPA$ vagrant ssh client1.test.local
Last login: Sat Mar 20 13:07:03 2021 from 10.0.2.2
[vagrant@client1 ~]$ kinit admin
Password for admin@TEST.LOCAL: 
[vagrant@client1 ~]$ klist
Ticket cache: KEYRING:persistent:1000:1000
Default principal: admin@TEST.LOCAL

Valid starting       Expires              Service principal
20.03.2021 13:08:38  21.03.2021 13:08:35  krbtgt/TEST.LOCAL@TEST.LOCAL
[vagrant@client1 ~]$ 
```

![Скриншот с сервера](/images/1.png)
