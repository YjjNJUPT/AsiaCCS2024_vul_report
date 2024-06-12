# Tracking of Default Settings Vulnerabilities of Home Router Features

This repo tracks the vulnerabilities discovered in our work<sup>[1]</sup>.

We tested the security of various features of 40 commercial off-the-shelf home routers, including IPv6, Wi-Fi security protocols, WPS, TLS, guest network, etc.
In total, we found 46 potential vulnerabilities, and 30 of them have been confirmed to be exploitable in the latest version by us.

We have reported all of confirmed vulnerabilities to manufacturers. Only 5 vulnerabilities have been fixed by manufacturers (D-Link and TP-Link respond very positively). Most manufacturers, especially Chinese manufacturers, have not responded to us. Some vulnerabilities are not accepted by manufacturers because they don't think it's a vulnerability. For example, guest network is not isolated from main network by default, but the manufacturer believes that it is not a vulnerability because users can isolate them by enabling an option (disabled by default).

The following vulnerabilities were submitted to CVE/CNVD and assigned a number. Most of the details have not been publicly disclosed yet due to the lack of disclosure from manufacturers.

CNVD/CVE ID  |  Vulnerability type  |  Model name  &  Affected version  |  Vulnerability Disclosure
  ----       |  ----                |  ----                             |  ----
CNVD-2023-59339 | Hard-coded WPS PIN | D-Link R15 <= v1.08B01 | https://supportannouncement.us.dlink.com/announcement/publication.aspx?name=SAP10330
CVE-2023-41603 | No IPv6 NAT and Firewall | D-Link R15 <= v1.08.02 | https://supportannouncement.us.dlink.com/announcement/publication.aspx?name=SAP10347
CVE-2023-41604 | No IPv6 NAT and Firewall | Tenda AX2 Pro <= V16.03.29.36 | 
CVE-2023-43852 | No IPv6 NAT and Firewall | TP-Link TL-WDR7650 <= 3.0.7 |
CVE-2023-43855 | No IPv6 NAT and Firewall | Netcore POWER 9S PRO <= V1.0.0.221114.103550 |
CVE-2023-50487 | No IPv6 NAT and Firewall | TP-Link TL-WR841N(US) v13 <= 180119 |
CVE-2023-43854 | Missing SSL Certificate Validation | Tenda AX12 Pro <= V16.03.20.17_cn and Tenda AX2 Pro <= V16.03.29.45_cn |
CVE-2023-50024 | Missing SSL Certificate Validation | Netcore N3 <= 3.0.5.59643 and Netcore N30 <= 1.0.1.230406.171444 |
CVE-2023-50025 | Missing SSL Certificate Validation | Ruijie X32 Pro <= 1.203.1614 |
CVE-2024-36755 | Missing SSL Certificate Validation | D-Link DIR-1950 <= 1.11B03 |
CVE-2024-36758 | Missing SSL Certificate Validation | H3C NX15 <= V100R012 | 
CVE-2024-36756 | Missing SSL Certificate Validation | Ruijie X32 PRO <= B11P226 |
CVE-2024-36757 | Missing SSL Certificate Validation | Xiaomi 4A <= 2.28.503 |
CVE-2024-36759 | Missing SSL Certificate Validation | ASUS RT-AC66U B1 <= 3.0.0.4_386_51685, ASUS TUF-AX5400 <= 3.0.0.4.388_24121 and ASUS TUF-AX3000 V2 <= 3.0.0.4.388_23785 |


[1] Junjian Ye, Xavier de Carné de Carnavalet, Lianying Zhao, Mengyuan Zhang, Lifa Wu, and Wei Zhang. 2024. Exposed by Default: A Security Analysis of Home Router Default Settings. In ACM Asia Conference on Computer and Communications Security (ASIA CCS ’24), July 1–5, 2024, Singapore, Singapore. ACM, NewYork, NY, USA, 17 pages. https://doi.org/10.1145/3634737.3637671
