### 4. Networking Tools

#### Task 4.1: Check Connectivity to google.com

```bash
ping google.com > ping_output.txt
```

Description: Logs the ping results to a file named `ping_output.txt`.

---

#### Task 4.2: Ping with 10 Packets

```bash
ping -c 10 google.com > ping_10_packets.txt
```

Description: Sends 10 packets to `google.com` and logs the results to `ping_10_packets.txt`.

---

#### Task 4.3: Ping with Packet Size 1000 Bytes

```bash
ping -s 1000 google.com > ping_large_packet.txt
```

Description: Logs ping results with a custom packet size of 1000 bytes to `ping_large_packet.txt`.

---

#### Task 4.4: Test Port 80 Connectivity to discord.com

```bash
telnet discord.com 80
```

Description: Tests connectivity to `discord.com` on port 80.

---

#### Task 4.5: Test SMTP Connectivity to smtp.gmail.com

```bash
telnet smtp.gmail.com 25
```

Description: Checks connectivity to the SMTP server on port 25.

---

#### Task 4.6: Fetch Content of discord.com

```bash
curl https://discord.com -o discord.html
```

Description: Saves the HTML content of `discord.com` to a file named `discord.html`.

---

#### Task 4.7: Fetch Content with Custom Header

```bash
curl -H "User-Agent: MyBrowser" https://google.com
```

Description: Sends a custom `User-Agent` header while fetching the content of `google.com`.

---

#### Task 4.8: List Active TCP Connections

```bash
netstat -t
```

Description: Lists all active TCP connections.

---

#### Task 4.9: Display Listening Ports

```bash
netstat -l
```

Description: Displays all ports in the listening state.

---

#### Task 4.10: Test Network Bandwidth (Client Mode)

```bash
iperf -c iperf-server.google.com
```

Description: Runs an `iperf` test in client mode to a remote server.

---

#### Task 4.11: Test Bandwidth (Server Mode)

```bash
iperf -s
```

Description: Starts an `iperf` server to listen for incoming connections.

---

#### Task 4.12: Check if Port 443 is Open on discord.com

```bash
nc -z discord.com 443
```

Description: Checks if port 443 is open on `discord.com` using `netcat`.

---

#### Task 4.13: Send Message to google.com on Port 12345

```bash
echo "Hello, Server!" | nc google.com 12345
```

Description: Sends the message "Hello, Server!" to `google.com` on port 12345 using `netcat`.

---

#### Task 4.14: Start HTTP Server on Port 8080

```bash
nc -l 8080 < index.html
```

Description: Serves `index.html` on port 8080.

---

#### Task 4.15: Query DNS on 8.8.8.8 for discord.com

```bash
telnet 8.8.8.8 53
```

Description: Manually queries the DNS server at `8.8.8.8` for the domain `discord.com`.

---
