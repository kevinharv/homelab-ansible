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