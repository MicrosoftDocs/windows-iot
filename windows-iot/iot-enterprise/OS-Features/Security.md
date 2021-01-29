---
title: Security
author: rsameser
ms.author: riameser
ms.date: 1/29/2020
ms.topic: article
ms.prod: windows-iot
ms.technology: iot
description: Learn about the Security features of Windows 10 IoT Enterprise.
keywords: IoT Enterprise, Security
---

# Security
Windows 10 IoT Enterprise comes with a host of [security offerings](https://docs.microsoft.com/windows/whats-new/ltsc/whats-new-windows-10-2019#security) that you can leverage to best fit your Windows 10 IoT Enterprise solution.

## Microsoft Security Response Center
The world is more connected today than it has ever been. Technology is wound deep into our lives and has become part of our routine. With great advances we have also seen a greater dynamic playing out between threat actors and the defenders. The [Microsoft Security Response Center (MSRC)](https://www.microsoft.com/msrc?rtc=1) is part of the defender community and on the front line of security response evolution. For over twenty years MSRC has been working to improve security for our customers, learning from both successes and failures. Time has only reasserted MSRC's commitment to better protect customers and the broader ecosystem.

MSRC's mission is to protect customers from being harmed by security vulnerabilities in Microsoft's products and services. By building your solution with Windows 10 IoT Enterprise, you have Microsoft Security Response Center's commitment towards security. Please review their [Security Update Guide](https://msrc.microsoft.com/update-guide/) to ensure your devices are up-to-date and secured.

## Comprehensive Security Features
Windows 10 IoT Enterprise, brings Enterprise security to your IoT devices.

Windows 10 IoT Enterprise is built on a 5-point comprehensive security platform:
1. [Device protection](#device-protection)
2. [Threat Resistance](#threat-resistance)
3. [Data Protection in Motion](#data-protection-in-motion)
4. [Cloud Security](#cloud-security)
5. [Response](#response)

## Device Protection
Windows Security provides the following built-in security options to help protect your device from malicious software attacks. Like they say, a strong defense, is a strong offense.

### Trusted Platform Module (TPM)​
[Trusted Platform Module (TPM)](https://docs.microsoft.com/windows/security/information-protection/tpm/trusted-platform-module-top-node) technology is designed to provide hardware-based, security-related functions. A TPM chip is a secure crypto-processor that is designed to carry out cryptographic operations. The chip includes multiple physical security mechanisms to make it tamper resistant, and malicious software is unable to tamper with the security functions of the TPM. Some of the key advantages of using TPM technology are that you can:
* Generate, store, and limit the use of cryptographic keys.
* Use TPM technology for platform device authentication by using the TPM’s unique RSA key, which is burned into itself.
* Help ensure platform integrity by taking and storing security measurements.

### Windows Device Health Attestation​
Modern malware is getting more and more sophisticated. Some of them, specifically bootkits, are capable of starting before Windows. [Device Health Attestation](https://github.com/ms-iot/iot-core-azure-dm-client/blob/master/docs/device-health-attestation.md) can be used to detect and remediate in the unlikely event where a device is infected. The device's firmware logs the boot process, and [Windows](https://docs.microsoft.com/windows-server/security/device-health-attestation) can send it to a trusted Health Attestation Server that can objectively assess the device's health.

### Secure Boot​
[Secure boot](https://docs.microsoft.com/windows-hardware/design/device-experiences/oem-secure-boot) is a security standard developed by members of the PC industry to help make sure that a device boots using only software that is trusted by the Original Equipment Manufacturer (OEM). When the PC starts, the firmware checks the signature of each piece of boot software, including UEFI firmware drivers (also known as Option ROMs), EFI applications, and the operating system. If the signatures are valid, the PC boots, and the firmware gives control to the operating system.

The OEM can use instructions from the firmware manufacturer to create Secure boot keys and to store them in the PC firmware. When you add UEFI drivers, you'll also need to make sure these are signed and included in the Secure Boot database.

For information on how the secure boot process works included Trusted Boot and Measured Boot, see [Secure the Windows 10 boot process](https://docs.microsoft.com/windows/security/information-protection/secure-the-windows-10-boot-process).

### BitLocker​
Wherever confidential data is stored, it must be protected against unauthorized access. Windows has a long history of providing at-rest data-protection solutions that guard against nefarious attackers, beginning with the Encrypting File System in the Windows 2000 operating system. More recently, [BitLocker](https://docs.microsoft.com/windows/security/information-protection/bitlocker/bitlocker-device-encryption-overview-windows-10) has provided encryption for full drives and portable drives. Windows consistently improves data protection by improving existing options and by providing new strategies. To learn more, see [BitLocker Overview and Requirements FAQ](https://docs.microsoft.com/windows/security/information-protection/bitlocker/bitlocker-overview-and-requirements-faq)

## Threat Resistance
We provide a security tools set for Windows to protected a wide range of threats against execution of unauthorized code and scripts, network and malware attacks. Effectively identifying, assessing, and remediating endpoint weaknesses is pivotal in running a healthy security program and reducing organizational risk. Threat and vulnerability management serves as an infrastructure for reducing organizational exposure, hardening endpoint surface area, and increasing organizational resilience.


### Windows Defender Firewall
[Windows Defender Firewall](https://docs.microsoft.com/windows/security/threat-protection/windows-firewall/windows-firewall-with-advanced-security) is a stateful host firewall that helps secure the device by allowing you to create rules that determine which network traffic is permitted to enter the device from the network and which network traffic the device is allowed to send to the network. Windows Defender Firewall also supports Internet Protocol security (IPsec), which you can use to require authentication from any device that is attempting to communicate with your device. When authentication is required, devices that cannot be authenticated as a trusted device cannot communicate with your device. You can also use IPsec to require that certain network traffic is encrypted to prevent it from being read by network packet analyzers that could be attached to the network by a malicious user.

* [Deployment Guide](https://docs.microsoft.com/windows/security/threat-protection/windows-firewall/windows-firewall-with-advanced-security-deployment-guide)
* [Best Practices](https://docs.microsoft.com/windows/security/threat-protection/windows-firewall/best-practices-configuring)

### Windows Defender
[Microsoft Defender for Endpoint](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection) is a unified platform for preventative protection, post-breach detection, automated investigation, and response. Defender for Endpoint protects endpoints from cyber threats, detects advanced attacks and data breaches, automates security incidents, and improves security posture.

## Data Protection in Motion
Data Protection covers control of data protection at rest, in transit, and via authorized access mechanisms. This includes discover, classify, protect, and monitor sensitive data assets using access control, encryption, and logging.

### X.509/TLS-Based Handshake and Encryption
Transport Layer Security (TLS), like Secure Sockets Layer (SSL), is an encryption protocol intended to keep data secure when being transferred over a network. [These articles](https://docs.microsoft.com/mem/configmgr/core/plan-design/security/enable-tls-1-2) describe steps required to ensure that Configuration Manager secure communication uses the TLS 1.2 protocol.


## Cloud Security
Microsoft Azure includes tools to safeguard data according to your company's security and compliance needs.

### Encryption at Rest
Encryption is the secure encoding of data used to protect confidentiality of data. The Encryption at Rest design uses symmetric encryption to encrypt and decrypt large amounts of data quickly according to a simple conceptual model:

* A symmetric encryption key is used to encrypt data as it is written to storage.
* The same encryption key is used to decrypt that data as it is readied for use in memory.
* Data may be partitioned, and different keys may be used for each partition.
* Keys must be stored in a secure location with identity-based access control and audit policies. Data encryption keys are often encrypted with a key encryption key in Azure Key Vault to further limit access.

In practice, key management and control scenarios, as well as scale and availability assurances, require additional constructs. Learn more about [Encryption at Rest concepts and components](https://docs.microsoft.com/azure/security/fundamentals/encryption-atrest).

### Azure Active Directory
The Azure Active Directory (Azure AD) enterprise identity service provides single sign-on and multi-factor authentication to help protect your users and their devices from 99.9 percent of cybersecurity attacks.
* [Azure Active Directory Documentation](https://docs.microsoft.com/azure/active-directory/)

### Key Vault
[Azure Key Vault](https://docs.microsoft.com/azure/key-vault/general/basic-concepts) is a cloud service for securely storing and accessing secrets. A secret is anything that you want to tightly control access to, such as API keys, passwords, certificates, or cryptographic keys. Key Vault service supports two types of containers: vaults and managed HSM pools. Vaults support storing software and HSM-backed keys, secrets, and certificates. Managed HSM pools only support HSM-backed keys. See [Azure Key Vault REST API overview](https://docs.microsoft.com/azure/key-vault/general/about-keys-secrets-certificates) for complete details.

### Policy-Based Access Control
The combination of Azure RBAC and Azure Policy provides full scope control in Azure.

There are a few key differences between [Azure Policy and Azure role-based access control (Azure RBAC)](https://docs.microsoft.com/azure/governance/policy/overview#azure-policy-and-azure-rbac). Azure Policy evaluates state by examining properties on resources that are represented in Resource Manager and properties of some Resource Providers. Azure Policy doesn't restrict actions (also called operations). Azure Policy ensures that resource state is compliant to your business rules without concern for who made the change or who has permission to make a change.

Azure RBAC focuses on managing [user actions](https://docs.microsoft.com/azure/role-based-access-control/resource-provider-operations) at different scopes. If control of an action is required, then Azure RBAC is the correct tool to use. Even if an individual has access to perform an action, if the result is a non-compliant resource, Azure Policy still blocks the create or update.

### IP-based Blocking
With the location condition in Conditional Access, you can control access to your cloud apps based on the network location of a user. The location condition is commonly used to block access from countries/regions where your organization knows traffic should not come from. More information about the location condition in Conditional Access can be found in the article, [What is the location condition in Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)

## Response
Microsoft has all the tooling to provide immediate support and assistance.  

### Device Management
Microsoft provides a whole suite of device management solutions to keep your devices safe and monitor activity at all times. Managing a device is now easier than ever on Windows 10 IoT Enterprise. There are multiple options that your organization can choose from in order to best manage your devices, such as Microsoft Intune, Endpoint Manager and 3rd party OMA-DM based management tools. OEMs can also select Azure Device Agent, which leaves it up to their customers to select the device management solution that fits them best.  

### Device Recovery
On the off chance something does go wrong, The Microsoft [Support and Recovery Assistant](https://www.microsoft.com/download/100607) works by running tests to figure out what's wrong and offers the best solution for the identified problem. It can currently fix Office, Office 365, Outlook, and Windows problems. If the Microsoft Support and Recovery Assistant can't fix a problem for you, it will suggest next steps and help you get in touch with Microsoft support.


## Additional resources
* [Azure Security Center](https://azure.microsoft.com/services/security-center/)
* [Azure Security Benchmark](https://docs.microsoft.com/azure/security/benchmarks/overview)
