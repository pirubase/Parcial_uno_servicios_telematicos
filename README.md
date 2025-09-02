# Parcial_uno_servicios_telematicos
este es el github del primer parcial
primera parte:
1. Configuración del servidor maestro (192.168.50.3)

 Archivos modificados:
 - /etc/bind/named.conf.local
     zone "empresa.local" {
    type master;
    file "/etc/bind/db.empresa.local";
    allow-transfer { 192.168.50.4; };
    also-notify    { 192.168.50.4; };
};

zone "50.168.192.in-addr.arpa" {
    type master;
    file "/etc/bind/db.192";
    allow-transfer { 192.168.50.4; };
    also-notify    { 192.168.50.4; };
};

- /etc/bind/db.empresa.local
    $TTL 3600
@   IN SOA ns.empresa.local. admin.empresa.local. (
        2025090102 ; serial
        3600       ; refresh
        900        ; retry
        1209600    ; expire
        300 )      ; minimum

    IN NS ns.empresa.local.

ns      IN A 192.168.50.3
esclavo IN A 192.168.50.4
www     IN A 192.168.50.3
api     IN A 192.168.50.3
cliente IN A 192.168.50.2
web     IN CNAME www

- /etc/bind/db.192
    $TTL 3600
@   IN SOA ns.empresa.local. admin.empresa.local. (
        2025090102 ; serial
        3600       ; refresh
        900        ; retry
        1209600    ; expire
        300 )      ; minimum

    IN NS ns.empresa.local.

2 IN PTR cliente.empresa.local.
3 IN PTR ns.empresa.local.
4 IN PTR esclavo.empresa.local.

2. Configuración del servidor esclavo (192.168.50.4)
