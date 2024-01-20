### Description
This dataset was generated from an oil and gas testbed that emulates a gas wellhead monitoring station for cybersecurity research and developing various anomaly detection techniques and machine learning models. It consists of a Remote Terminal Unit (RTU) receiving sensor readings from temperature and pressure sensors, a flow meter, 2 solenoid valves acting as an emergency shutdown valve and flare relief valve. The RTU is polled intermittently by a Human Machine Interface (HMI) to constantly display the pressure, temperature, and flow readings, as well as display the status of the valves (whether in open of closed state). Commands can be sent to alter the valve state through the HMI and the communications protocol is ModbusTCP.

The testbed setup can be viewed here:
![testbed](https://github.com/abusadiqmohd/ICS_testbed_pcaps/assets/35866933/0cb275fe-180c-49c2-b454-f9eab22b95e4)


### Citation Request
Mohammed, A. S., Anthi, E., Rana, O., Saxena, N., & Burnap, P. (2023). Detection and mitigation of field flooding attacks on oil and gas critical infrastructure communication. Computers & Security, 124, 103007.

### Dataset File Captures (Pcap Files)
1. Benign_capture (no attacks, clean operations depicting normal state)
2. mitm_attacks (pcap files containing Man-in-the-Middle attacks)
3. syn_flooding_attacks (pcap files containing ddos syn flooding attacks)
4. field_flooding_attacks (pcap files containing field flooding attacks)

File naming criteria

For each file, the naming format is:
[attack]_[attack duration]_[capture duration].pcapng

Example:
fieldflood_31m_1h.pcapng refers to a capture for a field flooding attack that lasted for 31 minutes over a 1 hour capture period.
