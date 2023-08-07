# Network Troubleshooting Guide

Follow these steps to troubleshoot network connectivity issues:

1. **Power On Devices:**
   - Ensure the following devices are powered on:
     - Device A (Member Server)
     - Device B (Workstation)
     - Device C (Web Server)
     - Device D (Router)

2. **Connect to Device B:**
   - Establish a connection to Device B.

3. **Ping Device A:**
   - Open the command prompt on Device B.
   - Send an ICMP echo request to ping Device A:
     ```cmd
     ping <IP_address_A>
     ```
   - If the ping is unsuccessful, there may be an issue with connectivity to Device A.

4. **Reconfigure Firewall on Device A:**
   - Access Device A.
   - Open the "Firewall & network protection" settings.
   - Click on "Allow an app through the firewall."
   - Locate "File and Printer Sharing" in the list of allowed apps.
   - Check the private box and click OK to allow the app through the firewall.
   - Return to Device B.

5. **Ping Device A Again:**
   - On Device B's command prompt, ping Device A again:
     ```cmd
     ping <IP_address_A>
     ```
   - This time, a successful ICMP echo request indicates that the firewall reconfiguration on Device A resolved the issue.

6. **Clear Command Prompt:**
   - Type `cls` to clear the command prompt screen.

7. **Trace Route to Device C (Web Server):**
   - Examine the route a packet will take to reach Device C (Web Server):
     ```cmd
     tracert <IP_address_C>
     ```
   
Follow these steps to diagnose and resolve network connectivity problems.

