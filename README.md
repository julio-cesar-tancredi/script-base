# script-base
Script Base para atividades do SENAI
enable
configure terminal
hostname (NOME DO EQUIPAMENTO)
enable password (SENHA)
enable secret (SENHA)
ip domain-name (NOME DO DOMÍNIO)
crypto key generate rsa general-key modulus (QUANTIDADE DE BITS)
line vty 0 15
transport input ssh
password (SENHA)
login
exit
banner motd "MENSAGEN"
line console 0
password (SENHA)
login
exit
service password-encryption
interface vlan 1
ip address [IP] [MÁSCARA]
no shutdown
exit
interface [fastethernet,gigabitethernet,vlan]
description [DESCRIÇÃO_DA_INTERFACE]
exit
interface [fastethernet,gigabitethernet,vlan]
description [DESCRIÇÃO_DA_INTERFACE]
exit
interface [fastethernet,gigabitethernet,vlan]
description [DESCRIÇÃO_DA_INTERFACE]
end
wr
exit
