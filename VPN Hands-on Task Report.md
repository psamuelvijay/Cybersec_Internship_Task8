# VPN Hands-on Task Report

## Objective
To understand VPNs' role in privacy and secure communication, set up a free VPN client, demonstrate hands-on usage, and analyze performance and privacy outcomes.

---

## 1. VPN Service Selection & Setup

- Chose ProtonVPN Free Tier due to its reputation for strong privacy and no-logs policy.
- Registered for a free account at protonvpn.com (email and password setup required).
- Downloaded the ProtonVPN installer for Windows.
- During setup, declined (unchecked) optional installations for Proton Mail, Drive, and Pass, as only the VPN client was required.
- Completed installation and launched the ProtonVPN app.

---

## 2. Connection & IP Verification

- Connected to the nearest available VPN server using the ProtonVPN application.
- Checked the public IP address on whatismyipaddress.com:
  - **With VPN:** IPv4 detected as `149.88.103.40`. No IPv6 address detected, showing proper IPv6 leak protection.
- Confirmed encrypted VPN tunnel before browsing and accessing other services online.

---

## 3. Speed Test Results

| State        | Download Speed | Upload Speed | Detected Public IP                           | Note                        |
|--------------|---------------|--------------|----------------------------------------------|-----------------------------|
| With VPN     | 59.6 Mbps     | 10.6 Mbps    | 149.88.103.40 (IPv4)                         | Good VPN download; IPv6 hidden |
| Without VPN  | 114.5 Mbps    | 0.10 Mbps    | 2405:201:c00d:7022:ec44:122b:9c4f:410d (IPv6)| No IPv4 detected            |

- Significant (~48%) drop in download speed and large increase in upload speed with VPN on.
- Hides the real IP (switches from IPv6 at home to remote IPv4 on VPN).

---

## 4. Browsing and Security Test

- Browsed multiple HTTPS websites; no connectivity issues were observed with VPN enabled.
- Gmail’s "Encrypted attachment" warning appeared for email attachments, indicating Gmail couldn't scan an encrypted file.
  - This warning is likely unrelated to VPN use and is a default Gmail behavior for encrypted/unknown files.

---

## 5. VPN Features, Benefits, and Limitations

### Encryption & Privacy Features

- ProtonVPN uses modern encryption (AES-256/OpenVPN, WireGuard).
- It enforces a strong no-logs policy and offers DNS leak protection, a kill switch, and default IPv6 leak-blocking.
- No IPv6 detection on the VPN connection confirms leak protection works as expected.

### Benefits

- Masks the device's real IP address and hides geographic location.
- Encrypts all traffic between the user and the VPN exit server, providing confidentiality on public and private networks.
- Circumvents geo-restrictions and access controls.

### Limitations

- Some speed loss (up to ~50% of direct connection in this case).
- Free VPNs offer fewer location/server choices.
- VPNs do not anonymize endpoint activities (e.g., websites visited can still track activity via cookies).

---

## Conclusion

Hands-on usage of ProtonVPN successfully demonstrated the principles and benefits of VPN use: privacy, data encryption, public IP masking, and network security. Speed reduction is expected and acceptable for everyday browsing but may impact large downloads or low-latency activities. VPNs are an important, but not complete, privacy tool.
