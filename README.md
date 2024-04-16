# Network Discovery Tool

This Bash script performs a ping sweep across a range of IP addresses in a local network. It iterates through all IP addresses within the specified range and sends a single ICMP echo request (ping) to each of them. The goal is to identify which IP addresses are active and responded to the ping, which can be useful for diagnosing connectivity issues or identifying active devices on the network.

## How to Use

1. **Specify the IP Range**: Modify the script to specify the desired IP range. By default, it scans the range from `0` to `254` in the last octet of the IP address.

2. **Run the Script**: Execute the script by running the Bash file in a terminal. Make sure you have the necessary permissions to execute the script.

   ```bash
   ./scan.sh [base_ip_address]
   ```
   Replace [base_ip_address] with the first three octets of the IP address range you want to scan.

3. **Review the Results**: After the script finishes executing, it will output a list of IP addresses that responded to the ping along with their respective Time to Live (TTL) values. This information can be useful for network analysis and troubleshooting.
