***
* IP
* DNS - mais famoso o BIND
* Firewall
* SSH
* [NFS](https://en.wikipedia.org/wiki/Network_File_System)
* [CUPS](https://en.wikipedia.org/wiki/CUPS) - servidor de impressão
* DHCP 
Um servidor DHCP (Dynamic Host Configuration Protocol) é um tipo de servidor que fornece automaticamente endereços IP e outras configurações de rede, como o gateway padrão e o servidor DNS, a dispositivos que se conectam à rede. Em vez de atribuir manualmente um endereço IP a cada dispositivo, o servidor DHCP automatiza esse processo e atribui um endereço IP disponível na rede.

* [Postfix](http://www.postfix.org/) - servidor de email
* OpenLDAP - servidor LDAP

|Comando|Descrição|
|---|---|
|dig| dns lookup |
|ping| ping de rede|
|ping6| ping IPv6|
|ifconfig| configurar ou visualizar a rede|
|host| dns lookup utility|
|route| configurar ou visualizar rotas|
|ip| substitui o ifconfig e o route `ip addr show` `ip route show`|
|netstat| imprime conexões de rede|




/etc/hosts
/etc/resolv.conf - utilizar resolvconf para editar este arquivo
