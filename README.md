## Полезные ссылки
- Disable systemd-resolve:
https://www.qualityology.com/tech/ubuntu-port-53-already-in-use-how-to-free-the-dns-port/#Edit-etc-systemd-resolved-conf-set-DNSStubListener-to-no

## Tips
Запретить доступ к DNS pi-hole в docker извне:

    iptables -I DOCKER-USER -i ens2 -p tcp --dport 53 -j DROP
