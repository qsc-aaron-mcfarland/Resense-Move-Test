# Core Redundancy Test Cases

## 10.a - IWS - Verify IWS device works with redundant core system

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a design with a redundant Core pair (active and backup).<br>3. Add an IWS component to the canvas.<br>4. IWS device is on the network, inventory item name matches device name in Configurator.<br>5. Deploy the design to the active Core. |
| **Steps** | 1. Verify the IWS device is in "OK" state on the active Core.<br>2. Verify sensor data is flowing from the IWS device.<br>3. Confirm the backup Core is in standby and aware of the IWS device. |
| **Expected Results** | 1. The IWS device operates normally with the redundant core system.<br>2. Sensor data flows correctly to the active Core.<br>3. The backup Core has the IWS device in its peripheral inventory. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Core Redundancy |

---

## 10.b - IWS - Verify IWS connects to backup core on active core failure

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design with redundant Core pair is deployed.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. IWS device is in "OK" state on the active Core.<br>5. Sensor data is flowing normally. |
| **Steps** | 1. Simulate an active Core failure (power off or network disconnect the active Core).<br>2. Wait for the backup Core to take over as active.<br>3. Observe the IWS device status on the new active Core.<br>4. Verify sensor data flow resumes. |
| **Expected Results** | 1. The backup Core takes over as the active Core.<br>2. The IWS device connects to the new active Core.<br>3. The IWS device reaches "OK" state without manual intervention.<br>4. Sensor data resumes flowing within a reasonable failover time. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Core Redundancy |

---

## 10.c - IWS - Verify IWS connects to backup core on graceful switchover

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Design with redundant Core pair is deployed.<br>3. IWS device is on the network, inventory item name matches device name in Configurator.<br>4. IWS device is in "OK" state on the active Core.<br>5. Sensor data is flowing normally. |
| **Steps** | 1. Initiate a graceful switchover from the active Core to the backup Core.<br>2. Wait for the switchover to complete.<br>3. Observe the IWS device status on the new active Core.<br>4. Verify sensor data flow. |
| **Expected Results** | 1. The graceful switchover completes successfully.<br>2. The IWS device connects to the new active Core.<br>3. The IWS device reaches "OK" state without manual intervention.<br>4. Sensor data resumes with minimal interruption. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Core Redundancy |
