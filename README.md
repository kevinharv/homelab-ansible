# TODO
- Configure Vagrantfile to replicate HL
- Complete devInv.yml
- Test main.yml against Vagrant environment
- Documentation
- Change docker group membership to be based on current users rather than hard coded

# Roles
- Docker
    - Jellyfin
    - XMLTV (OTA Guide Feed)
- OpenVPN
- GNS3
- Minecraft Servers
    - Vanilla (PaperMC)
    - Modded (various)


# Steps for Use
1. Deploy Hosts
1. Configure Connectivity
1. Add to Inventory
1. Run main.yml playbook

## Docker Configuration


## Minecraft Configuration
Service User: minecraft
Service Group: minecraft
Working Directory: /opt/minecraft/server

OLD:
ExecStart=java -Xmx1024M -Xms1024M -jar /opt/minecraft/server/server.jar nogui

ausearch -c 'systemd' --raw | audit2allow -M my-systemd
semodule -X 300 -i my-systemd.pp



kubeadm join 10.0.2.15:6443 --token f06pm7.a1zyvbahju9y9s8r \
        --discovery-token-ca-cert-hash sha256:a9a5ba7f9b52e1bd4412be10c89f140d988e87853753c2307a86c849ff6cfa6b