# QPM (Q-SYS Peripheral Manager) Management Test Cases

## 04.p - IWS - Verify hostname can be changed via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Navigate to the IWS device in QPM.<br>2. Locate the hostname field.<br>3. Change the hostname to a new value (e.g., "IWS-LobbyA").<br>4. Save/apply the change.<br>5. Verify the hostname update takes effect. |
| **Expected Results** | 1. The hostname field is editable.<br>2. The new hostname is accepted and saved.<br>3. The device is accessible by its new hostname after the change.<br>4. Q-SYS Designer reflects the updated hostname. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.q - IWS - Verify network settings can be configured via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Navigate to the IWS device network settings in QPM.<br>2. Configure a static IP address, netmask, and gateway.<br>3. Save/apply the changes.<br>4. Verify the device is reachable at the new IP address.<br>5. Optionally configure a static route and verify connectivity. |
| **Expected Results** | 1. IP address, netmask, and gateway fields are editable.<br>2. Changes are accepted and applied.<br>3. The device is reachable at the new network configuration.<br>4. Static routes, if configured, function correctly.<br>5. Q-SYS Designer can still communicate with the device at the new address. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.r - IWS - Verify NTP settings can be configured via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials.<br>4. An NTP server is available on the network. |
| **Steps** | 1. Navigate to the IWS device NTP settings in QPM.<br>2. Configure the NTP server address.<br>3. Save/apply the changes.<br>4. Verify the device synchronizes time with the configured NTP server. |
| **Expected Results** | 1. The NTP server field is editable.<br>2. The configuration is accepted and saved.<br>3. The device clock synchronizes with the NTP server.<br>4. Time synchronization status is visible in QPM. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.s - IWS - Verify device certificate management via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Navigate to the IWS device certificate management section in QPM.<br>2. Generate a Certificate Signing Request (CSR).<br>3. Verify the CSR is generated successfully.<br>4. Install a signed certificate on the device.<br>5. Verify the certificate is active. |
| **Expected Results** | 1. CSR generation completes without error.<br>2. The CSR contains correct device information.<br>3. A signed certificate can be installed successfully.<br>4. The device uses the installed certificate for secure communication.<br>5. Certificate status is visible in QPM. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.t - IWS - Verify secure communication management via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Navigate to the secure communication management section in QPM.<br>2. Verify TOFU (Trust On First Use) behavior for initial connection.<br>3. Verify the device appears in the trusted devices list after acceptance.<br>4. Move a device to the declined list and verify communication is blocked.<br>5. Verify rollover behavior when a device certificate changes. |
| **Expected Results** | 1. New devices appear in the pending list on first connection.<br>2. Accepting a device moves it to the trusted list and enables communication.<br>3. Declining a device blocks communication.<br>4. Certificate rollover is handled gracefully without manual intervention (or with appropriate prompts).<br>5. Trusted, pending, and declined lists are correctly maintained. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.u - IWS - Verify 802.1X management via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials.<br>4. An 802.1X-capable switch and RADIUS server are available on the network. |
| **Steps** | 1. Navigate to the 802.1X settings in QPM for the IWS device.<br>2. Enable 802.1X port-based authentication.<br>3. Configure the EAP method and credentials.<br>4. Save/apply the changes.<br>5. Verify the device authenticates successfully on the switch port. |
| **Expected Results** | 1. 802.1X settings are configurable in QPM.<br>2. The device successfully authenticates to the RADIUS server.<br>3. The switch port transitions to an authorized state.<br>4. Network communication continues normally after authentication.<br>5. Authentication status is visible in QPM. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.v - IWS - Verify security policy management via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Navigate to the security policy settings in QPM for the IWS device.<br>2. Configure password requirements (minimum length, complexity, etc.).<br>3. Configure session settings (timeout, maximum sessions, etc.).<br>4. Save/apply the changes.<br>5. Verify the new policies are enforced. |
| **Expected Results** | 1. Password requirement settings are editable and saved.<br>2. Session settings are editable and saved.<br>3. A password that does not meet requirements is rejected on next password change.<br>4. Sessions time out according to the configured policy.<br>5. Policy changes persist across device reboots. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.w - IWS - Verify system log and state download via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Navigate to the system log/diagnostics section in QPM for the IWS device.<br>2. Initiate a system log download.<br>3. Initiate a system state download.<br>4. Verify the downloaded files. |
| **Expected Results** | 1. System log downloads successfully as a readable file.<br>2. System state downloads successfully.<br>3. The log contains relevant device events and timestamps.<br>4. The system state file contains current device configuration and status information. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.x - IWS - Verify device reboot via QPM

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials.<br>4. Design is deployed and IWS device is in "OK" state. |
| **Steps** | 1. Navigate to the device management section in QPM for the IWS device.<br>2. Initiate a device reboot.<br>3. Confirm the reboot if prompted.<br>4. Wait for the device to come back online.<br>5. Verify device status in QPM and Q-SYS Designer. |
| **Expected Results** | 1. The reboot command is accepted.<br>2. The device goes offline temporarily.<br>3. The device comes back online within a reasonable time.<br>4. The device returns to "OK" state in Q-SYS Designer without manual intervention.<br>5. All previous configuration is retained after reboot. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |

---

## 04.y - IWS - Verify QPM re-authentication after password change

| Field | Details |
|---|---|
| **Preconditions** | 1. Open Q-SYS Peripheral Manager (QPM) in a web browser.<br>2. IWS device is commissioned and accessible.<br>3. Log in to QPM with valid credentials. |
| **Steps** | 1. Change the IWS device password via QPM or device web interface.<br>2. Attempt to access the device in QPM after the password change.<br>3. Observe the authentication prompt. |
| **Expected Results** | 1. QPM prompts the user to re-enter credentials after the password change.<br>2. Entering the new password restores access to the device.<br>3. No authentication faults are shown in Configurator (Configurator does not authenticate).<br>4. The device remains functional and connected to the Core. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > QPM Management |
