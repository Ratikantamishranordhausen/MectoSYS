\*\*26.05.2026

1: Configuration of the ring topology S7-1500 PLC as master and Festo CMMT-ST as slave. Tested and working fine.
2: Started working with SCALANCE XC208G, set to factory default as I ordered a used SCALANCE from Industry Mall. Configured basic settings and added to the TIA portal, but the configuration change was not loading.
3: I tried several ways, name and IP are ok, device is going online, HTTPS authentication OK, HTTPS server enabled, SINEMA configuration interface enabled.
4: Updated firmware from 4.3 to 4.4, still not working. So, decided to work currently with WBM and CLI.


\*\*27.05.2026

1: Mounted the Servo motor in a linear axis, printed a few 3D print part for mounting. Tested with the servo working fine.
2: Designed HMI for controlling the basic servo operations JOG, Positioning, with specified position and velocity. Calculated accel, decel.


\*\*28.05.2026
1: Configured Scalance with basic configuration, set up the user, SSH connection, and understood the concept of SSH, telnet, HTTP and HTTPS.


\*\*02.06.2026
1: Due to cost constraints, the pick and place module, along with one conveyor, was removed from the design. The current rev is 1.
2: Conveyor design finalised and shared procurement document with the university purchase team.


**05.06.2025
1: Configured the system time in scalance, created a NTP server using raspberry pi and sync the scalance with the NTP server and configured PTP for the servo drive.


**06.06.2026
1:Configured a SFTP server using raspberry pi and tested the setup, saved the config and other files in server periodically and factory reset the scalance and when connect to network the last backup transfered from SFTP to scalance.
2: VLAN configuration done for IT management and OT components. VLAN 10 and 20.


**07.06.2026
1: Tested ring redudency with scalance and understood the complete concept of ring redudency, standby, multi ring communication etc.
2: Using raspberry pi communicated to the scalance using SNMP and got port details and other details from scalance using SNMP V3.


**18.06.2026
1: Received ScalanceS615, S7-1215C and IOT2050 unit. 
2: Configured all the modules, downloaded a sample program on s7-1215C PLC, configured the parameters in ScalanceS615(Disabled non secure lines like Telnet, HTTP and configured other setting), configured the parameter of IOT2050.

**19.06.2026
1: Configured the Rpi as router, connected the Rpi to my room wifi and using ethernet connected to IOT2050, configured and performed update.
2: Tried to install siemens example os in IOT 2050 and in mid way the transfer got cancelled and the device is not loading. After going through several website came to know its a typical firmware issue.
3: Ordered USB to TTL UART 3.3V cable to trobleshoot.

**09.07.2026 - 10.07.2026
1: Received the USB to TTL UART cable, connected to check what happening in bootloader. The device is not getting any suitable OS.
2: Installed example os V1.1.1 in a SD card and rebooted it worked.
3: Installed firmware V1.1.1 from V1.0.0 and it cant directly upgrade to V1.6.3 the current available version.
4: Upgraded to V1.6.3 from V 1.1.1 and installed example os V1.6.3.

**11.07.2026 - 12.07.2026
1: Installed Uaexpert, configured OPC UA server on s7-1215C and performed a test using uaexpert as client.
2: Installed nodered opcua on IOT 2050 and configured the OPC UA communication it was easy it took 2 hour for me to show a value in dashboard but it took me 2 days to understand the configured a secure sign and encrypt communication.
3: Finally configured a secure OPC UA communication.
4: Configured MQTT in node red and send the tag to digital ocean droplet.
5: Configured NTP and sync all devices to NTP sever.

**13.07.2026
1: Received the mechanical parts, started mechanical assembly.

**16.07.2026
1: 3d printed all the small parts.