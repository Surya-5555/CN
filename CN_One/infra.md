-   **ISP (Internet Service Provider):** Companies like Comcast, AT&T, or Verizon are your gateway to the internet. They provide you with a modem/router.
-   **Local vs. Global IP:** All the devices connected to your home modem (your phone, laptop, smart TV) share the same public/global IP address with the outside world. Internally, however, they each have a unique local IP address (e.g., `192.168.1.5`).
-   **DHCP (Dynamic Host Configuration Protocol):** This is the system that automatically assigns those unique local IP addresses to all devices on your network.
-   **NAT (Network Address Translation):** Your router acts as a traffic director using NAT. When a request goes out, the router notes which local device sent it. When the response comes back to your single global IP address, NAT directs it to the correct device.

### Ports: The Application's Doorbell

An IP address gets data to the right *device*, but what about the right *application* on that device? This is where ports come in.

Ports are 16-bit numbers that function like a specific door or endpoint for an application on your device. Since they are 16-bit, there are **2^16 = 65,536** possible port numbers.

They are divided into ranges:

-   **Well-Known Ports (0 - 1023):** Reserved for standard, essential services. You can't use them for your own applications.
    -   **Port 80:** Used for standard HTTP web traffic.
-   **Registered Ports (1024 - 49152):** Registered for specific, well-known applications.
    -   **Port 1433:** Microsoft SQL Server.
    -   **Port 27017:** MongoDB database.
-   **Dynamic/Private Ports (49153 - 65535):** The remaining ports that applications can use dynamically.

## The Physical Stuff: Cables, Waves, and Speed

### Internet Speed

Internet speed is measured in **bits per second**.

-   **1 kbps (kilobits per second):** 1,000 bits per second.
-   **1 mbps (megabits per second):** 1,000,000 bits per second.
-   **1 gbps (gigabits per second):** 1,000,000,000 (10^9) bits per second.

### How Computers are Connected

Communication between computers happens in two primary ways:

1.  **Guided Media (Physical Wires):** Data is sent through physical cables.
    -   **Optical Fibre & Coaxial Cables:** These are the backbones of the internet. To connect countries and continents, massive submarine cables are laid on the ocean floor. You can visualize this on a Submarine Cable Map. This massive infrastructure is controlled by large corporate and government entities, while regional connectivity is often handled by local providers and startups.

2.  **Unguided Media (Wireless):** Data is transmitted through the air.
    -   **Radio Waves:** Used for WiFi, Bluetooth, 3G, 4G, and 5G.
    -   **Satellites:** While we have a vast network of underwater wires, satellites play a crucial role. They are essential for providing internet access to remote locations where laying cable is impossible. Although fiber optic cables generally offer lower latency (less delay), satellites provide critical global coverage.