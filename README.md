# Домашнее задание к занятию 10.1 «Keepalived/vrrp»

---

### Задание 1

Разверните топологию из лекции и выполните установку и настройку сервиса Keepalived. 

```
vrrp_instance test {

state "name_mode"

interface "name_interface"

virtual_router_id "number id"

priority "number priority"

advert_int "number advert"

authentication {

auth_type "auth type"

auth_pass "password"

}

unicast_peer {

"ip address host"

}

virtual_ipaddress {

"ip address host" dev "interface" label "interface":vip

}

}

```

*Пришлите скриншот рабочей конфигурации и состояния сервиса для каждого нода.*

#### Ответ:  

Нода 1  
![Скрин](https://github.com/Karhq/10.1_hw_keepalived/blob/main/Node_1_1.png)  
![Скрин](https://github.com/Karhq/10.1_hw_keepalived/blob/main/Node_1_2.png)  

Нода 2  
![Скрин](https://github.com/Karhq/10.1_hw_keepalived/blob/main/Node_2_1.png)  
![Скрин](https://github.com/Karhq/10.1_hw_keepalived/blob/main/Node_2_2.png)  

