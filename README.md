# Ansible Role ProtonVPN
This is an Ansible role that installs ProtonVPN on Linux. It uses the RPM/Deb repository so this should work on any Debian- or Red Hat derived distribution.

Tested on Fedora 36 and Ubuntu 22.04, should work on any Linux distribution that the ProtonVPN RPM/Deb repository supports.

## Requirements

### Base requirements
None  

## Variables
| Variable | Default | Description |
|----------|---------|-------------|
| `protonvpn_install_gui` | `false` | Whether to install the GUI utility. |
| `protonvpn_user` | `{{ ansible_user_id }}` | User to configure ProtonVPN for. |
| `protonvpn_configure_user` | `true` | Whether to place a configuration file for ProtonVPN |
| `protonvpn_default_protocol` | `udp` | Default protocol to use. Valid options are: `[udp, tcp]` |
| `protonvpn_killswitch` | `false` | Whether to enable the killswitch. |
| `protonvpn_dns_custom` | `false` | Whether to use custom DNS servers. |
| `protonvpn_dns_servers` | `[]` | List of DNS servers to use. |
| `protonvpn_netshield` | `false` | Whether to enable the NetShield. |
| `protonvpn_secure_core` | `false` | Whether to enable Secure Core. |
| `protonvpn_vpn_accelerator` | `true` | Whether to enable VPN Accelerator. |
| `protonvpn_alt_routing` | `true` | Whether to enable Alternative Routing. |
| `protonvpn_moderate_nat` | `false` | Whether to use Moderate NAT. |
| `protonvpn_non_standard_ports` | `false` | Whether to allow using non-standard ports. |

