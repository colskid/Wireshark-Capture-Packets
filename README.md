# Wireshark: Capture Packets

![Imgur](https://i.imgur.com/pZhPuJQ.jpg) 

Welcome to the "Wireshark for Beginners: Capture Packets" project! This repository aims to provide step-by-step guides for installing, setting up, and using Wireshark on Ubuntu. Whether you're new to packet analysis or looking to refresh your skills, this project will help you learn how to effectively capture and analyze network traffic using Wireshark.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Capturing Packets](#capturing-packets)
- [Detecting HTTP and HTTPS Packets](#detecting-http-and-https-packets)
- [Detecting IP Addresses in Packets](#detecting-ip-addresses-in-packets)
- [Contributing](#contributing)

## Introduction

Wireshark is a powerful and popular open-source network protocol analyzer. It allows you to capture and examine the data traveling back and forth on your network. In this project, you'll learn how to install Wireshark on an Ubuntu system, capture packets, and use display filters to detect specific types of packets.

## Installation

Follow these steps to install Wireshark on Ubuntu:

1. Update the package list:

   ```bash
   sudo apt update
   ```
2. Install Wireshark:

  ```bash
  sudo apt install wireshark
  ```
3. Add your user to the `wireshark` group to capture packets without needing root priveledges:

  ```sh
  sudo usermod -aG wireshark $USER
  ```

4. Log out and log back in to apply the group changes.

## Capturing Packets

Learn how to capture packets using Wireshark: <br><br>

1. Open Wireshark from the application menu or run wireshark in the terminal.

2. Select the network interface you want to capture packets from.

3. Click the "Start" button to begin capturing packets.

4. Capture packets for a specific duration or until you have enough data.

## Detecting HTTP and HTTPS Packets

Use display filters to detect HTTP and HTTPS packets: <br><br>

1. In Wireshark, go to the "Display Filter" field.

2. Enter http to filter for HTTP packets or tls to filter for TLS (HTTPS) packets.

3. Wireshark will display only the packets that match your filter.

## Detecting IP Addresses in Packets 

Use display filters to detect IP addresses in packets:<br><br>

1. In Wireshark, go to the "Display Filter" field.

2. Enter ip.addr == x.x.x.x where x.x.x.x is the IP address you want to filter.

3. Wireshark will display packets involving the specified IP address.

## Contributing 
Contributions to this project are welcome! If you find any issues or want to enhance the project, feel free to submit a pull request.
