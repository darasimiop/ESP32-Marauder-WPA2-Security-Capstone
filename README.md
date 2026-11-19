# ESP32 Marauder WPA2 Security Capstone

Washington State University · CptS 432 · 2025

I built and tested an ESP32-based wireless security prototype in an instructor-authorized lab. The project covered hardware assembly, firmware setup, fault isolation, packet analysis, and technical reporting.

## What I accomplished

- Assembled and soldered the ESP32, display, and microSD hardware, then flashed the Marauder firmware and checked boot and serial connectivity.
- Troubleshot intermittent storage and capture issues. My final report documents inspecting and reworking solder joints on the microSD header and verifying that the card mounted afterward.
- Examined WPA2 authentication traffic and distinguished incomplete captures from a complete EAPOL exchange.
- Documented that an initial offline password assessment returned no match and that a subsequent assessment recovered the lab passphrase. The result applies to the authorized lab configuration.
- Wrote a final report and prepared a presentation explaining the build, test results, and wireless security implications.

## Tools

| Tool | Role |
| --- | --- |
| ESP32 and Marauder firmware | Wireless test prototype |
| esptool and PuTTY | Firmware flashing and serial validation |
| Multimeter and microscope | Hardware inspection and troubleshooting |
| Wireshark | Packet and EAPOL analysis |
| cap2hashcat and Hashcat | Lab evidence conversion and offline password assessment |

## What I learned

An incomplete capture can reflect a collection problem. A completed assessment with no match is bounded by what was tested. Checking collection and analysis separately helped me explain why the early runs failed and what the successful run demonstrated. The lab also showed why strong, unique passphrases matter for WPA2-Personal networks.

For SOC analyst work, the most relevant skills are checking evidence quality, isolating technical faults, and communicating what the evidence supports.

[Read the lab findings and limitations](docs/lab-findings.md)
