# ICS Security Assessment Project

ABC Plant Tour
Explore the critical infrastructure and cybersecurity posture of a ABC power plant.
Welcome to ABC Plant Tour
Welcome to our virtual tour of a ABC power plant, where we'll explore its critical infrastructure and assess its cybersecurity posture.

Click this sample [here](http://www.google.com)

This journey will take us from the plant's exterior to the heart of its operations, providing an in-depth look at potential vulnerabilities and security practices.

## Step 1: Entering the Plant

Our tour begins at the main entrance of the power plant, where a vigilant security guard ensures that only authorized personnel enter the premises.
Physical security is the first line of defense in protecting critical infrastructure from unauthorized access.

## Step 2: Inside the Plant
As we move inside the plant, we are surrounded by the powerful hum of motors and pumps—the beating heart of the power generation process. 
These machines are crucial, but their security also depends on protecting the systems that control them.
Here, we see an engineer diligently monitoring the process through a field Human-Machine Interface (HMI).
HMIs are vital for real-time control, but they also present potential entry points for cyber threats if not adequately secured.

   Step 3: Control Room Security

Access to the control room is restricted and requires a smart card, highlighting the importance of access control in protecting sensitive operations. Let's step inside.
Within the control room, operators manage the Supervisory Control and Data Acquisition (SCADA) and Distributed Control Systems (DCS), which are the brains behind the plant's operations.
Securing these systems is paramount to maintaining operational integrity.
Field technicians are also busy ensuring that other critical systems function smoothly. 
The collaboration between the control room and field technicians is crucial for seamless operations, but it also necessitates strong cybersecurity practices across all interfaces.

Step 4: Maintenance and Engineering Room

Managers are responsible for overseeing maintenance activities, ensuring that field permits are approved, and maintaining compliance. 
Proper documentation and authorization are essential to avoid introducing risks during maintenance.

Now, we enter the engineering room, where instrumentation engineers work on engineering workstations to modify logic and ensure the safe operation of machines.
Their work is critical, but we notice something concerning—several engineering stations have been left unattended with systems still open. 
This oversight can expose sensitive systems to unauthorized access, emphasizing the need for strict cybersecurity policies.
Additionally, the cables from these desktops are not properly arranged, and USB ports are easily accessible. 
These physical vulnerabilities could be exploited to introduce malware or extract sensitive data.

Step 5: Server Room Security

Next, we use our smart card to access the server room, where the plant's critical networking and server infrastructure is housed. 
Robust access controls are crucial in this highly sensitive area.
Inside, we see a vast array of networking equipment and servers operating within cabinets. However, some cabinets have been left open and unlocked, posing a significant security risk. 
A more concerning issue is the presence of sticky notes with usernames, passwords, and other sensitive details pasted on servers and switches. 
This practice is a glaring security lapse that could easily be exploited.
On a positive note, we observe that the Programmable Logic Controller (PLC) rack is well maintained and in excellent condition, reflecting a commitment to securing critical control components.

Step 6: Security Monitoring and Final Measures

Physical security measures are also in place, as evidenced by the operational CCTV cameras installed throughout the plant. 
These cameras play a vital role in monitoring the plant's security.
Lastly, we ensure that the emergency and fire suppression systems are active, providing a final layer of safety for both personnel and critical infrastructure in case of an incident.  

Conclusion
As we conclude our tour, the view reminds us of the vast and complex nature of this facility. 
Ensuring the cybersecurity of such an operation is a continuous effort that requires vigilance, strong policies, and proactive measures

Materials 
All materials required for conducting risk assessment are.
Risk Assessment Template 
Invenyory List
Vulnerability List
Network Architecture

![image alt](https://github.com/funkecity/ICS-Security-Assessment-Project/blob/460845846ac362766bee09ee5f2832d36cd65da7/ABC%20Plant%20Archtecture.docx)
ABC Plant Network Architecture Overview
Introduction

The attached ABC Plant Network Diagram represents the layered architecture of the industrial control system (ICS) environment, based on the Purdue Model for ICS security. 
This structure segregates operational technology (OT) and information technology (IT) networks to ensure security, efficiency, and resilience.
Network Segmentation & Levels

    Level 4 (Enterprise Network)
        Workstations, business applications, and domain controllers for corporate IT functions.
        Direct internet connectivity for external access and enterprise-wide applications.

    Level 3.5 (DMZ - Industrial Demilitarized Zone)
        Enterprise AD Replica, Patch Management, and Remote Access services.
        Acts as a buffer between enterprise IT and OT environments.

    Level 3 (Operational Management Network)
        Hosts critical services like Historian, Database Servers, Domain Controllers, and Application Servers.
        Engineering Workstations (EWS-1, EWS-2) used for system administration.

    Level 2 (Supervisory Control Network)
        Supervisory Control and Data Acquisition (SCADA) systems.
        Human-Machine Interfaces (HMI-1, HMI-2) for process visualization and control.
        Historian-1 for logging real-time industrial process data.

    Level 1 (Control Network)
        Programmable Logic Controllers (PLCs) manage automated control functions.
        Communication through industrial switches (SW-1, SW-2).

    Level 0 (Physical Process Layer)
        Actuators, sensors, and field devices executing plant operations.
        Remote Terminal Units (RTU-1, RTU-2) interfacing with PLCs.
        Network Time Protocol (NTP) synchronization for accurate process control.
        Uninterruptible Power Supply (UPS) ensuring system availability.

Security Considerations
    Firewalls (FW-1, FW-2) separate IT and OT environments, preventing unauthorized access.
    Restricted Access to critical components via industrial switches.
    Remote Access Control through a secured gateway at Level 3.5.
    Cybersecurity Monitoring with layered segmentation to reduce attack surfaces.

Observation
The ABC Plant Network Architecture is designed with security best practices in mind, ensuring robust isolation between enterprise IT and OT infrastructure. 
Implementing proper access controls, network monitoring, and segmentation enhances both cybersecurity and operational efficiency.


![image alt](https://github.com/funkecity/ICS-Security-Assessment-Project/blob/fe2fcd97292d99be960387cf1b3729707ee5bd8e/ABC%20Plant%20Asset%20Inventory.xlsx)
ABC Plant Asset Inventory Overview

This document provides a high-level summary of the critical assets at ABC Plant, detailing their types, locations, and cybersecurity considerations.
1. Asset Categories

The plant's infrastructure consists of various asset types, including:

    Programmable Logic Controllers (PLCs) – Essential for process automation and control.
    Human-Machine Interfaces (HMIs) – Facilitate real-time monitoring and interaction with plant processes.
    SCADA Systems – Centralized monitoring and control for plant operations.
    Networking Equipment & Servers – Support data communication and processing.

2. Critical Assets and Locations

The plant consists of multiple critical assets distributed across different operational areas:

    Hydrogen Plant
        PLCs (Siemens S7-1200) – Control hydrogen production.
        HMIs (Rockwell PanelView) – Operator interface for hydrogen systems.
        SCADA System (Schneider SCX-5000) – Supervisory control for hydrogen processes.

    Water Treatment
        PLCs (Mitsubishi MELSEC iQ-R) – Control water treatment processes.
        HMIs (Siemens SIMATIC HMI) – Operator interface for water treatment.

    Control Room
        Hosts key operational assets, including PLCs, SCADA, and HMIs.
        Houses networking infrastructure such as switches, servers, and firewalls.

3. Cybersecurity Considerations

    Access Controls: Restricted access to control systems (smart cards required for entry).
    Network Security: PLCs, SCADA, and HMIs have defined IP addresses and are segmented for security.
    Physical Security: Equipment is housed in secured locations, though some vulnerabilities (unlocked cabinets, sticky notes with passwords) were identified.
    Firmware & Software Updates: Regular maintenance schedules ensure up-to-date firmware.
    Incident Readiness: Fire suppression systems and CCTV monitoring in place.

4. Maintenance & Compliance

    Maintenance Frequency: Assets have predefined schedules, such as quarterly or monthly checks.
    Last Maintenance Dates: Regular inspections ensure system reliability and security.

5. Key Security Risks

    Unattended Engineering Stations: Risk of unauthorized access.
    USB Accessibility: Potential for malware introduction.
    Open Server Cabinets: Exposes critical network infrastructure to physical tampering.
    Credential Handling Issues: Sticky notes with login credentials observed.

Obervation
The ABC Plant relies on a range of critical infrastructure assets for operations. 
Ensuring cybersecurity across these systems requires strict access controls, regular maintenance, and strong security policies to mitigate risks.

#  ABC Plant Vulnerabilities Report Overview

- Identified vulnerabilities in PLCs, HMIs, and OT devices
- Issues include outdated firmware, weak passwords, lack of encryption, unpatched software, and default credentials
- CVSS scores range from High to Critical
- Potential impacts: system malfunction, unauthorized access, data manipulation
- Mitigation: firmware updates, strong password policies, encryption (TLS/SSL), patch management, credential changes

  # ABC Plant Risk Assessment Summary

- **Assessed Zones:** Level 0 (Sensors), Level 1 to 3.5 (PLCs,HMI,NTP,FIREWALL,RTU,REMOTE SERVER EWS)
- **Threat Scenarios:** Internal (disgruntled employees), external (unauthorized access, Modbus command injection)
- **Key Vulnerabilities:** Lack of physical security controls, vulnerable communication protocols (e.g., Modbus)
- **Potential Consequences:** False sensor readings, process disruptions, safety hazards
- **Risk Ratings:** Vary from moderate to high based on impact and likelihood
- **Mitigations:** Physical security enhancements, strong authentication for Modbus, encrypted communication protocols
- **Recommendations:** Regular security audits, implementation of secure protocols, monitoring access controls


