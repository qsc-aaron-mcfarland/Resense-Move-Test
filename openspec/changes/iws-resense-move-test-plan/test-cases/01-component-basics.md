# Component Basics Test Cases

## 01.a - IWS - Verify component available in inventory

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design. |
| **Steps** | 1. In Left Sidebar > Inventory, click the "+" (Add) button in the toolbar.<br>2. In the Add to Inventory dialog, select the "Sensors" category on the left.<br>3. Locate "Intelligent Workspace Sensor" in the list on the right. |
| **Expected Results** | 1. The "Intelligent Workspace Sensor" appears in the Sensors list with description "Environmental sensor and human presence detector".<br>2. The component can be selected and added to the inventory. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.b - IWS - Add component to schematic via drag and drop

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design. |
| **Steps** | 1. In Left Sidebar > Inventory, click the "+" (Add) button in the toolbar.<br>2. In the Add to Inventory dialog, select the "Sensors" category.<br>3. Select "Intelligent Workspace Sensor" and click OK/Add.<br>4. The component is added to the Inventory tree; drag it from the Inventory onto Center Workspace > Canvas. |
| **Expected Results** | 1. The IWS component node appears on the canvas.<br>2. The component shows default name label (e.g., "IWS 1").<br>3. Input and output pins are visible on the component node. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.c - IWS - Verify default component properties

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Open Right Sidebar > Properties drawer.<br>3. Review all default property values. |
| **Expected Results** | 1. Component name defaults to "IWS 1" (or next available number).<br>2. All property fields display their default values.<br>3. No validation errors are shown. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.d - IWS - Rename component

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Open Right Sidebar > Properties drawer.<br>3. Change the component name to "Conference Room Sensor".<br>4. Click away to confirm the change. |
| **Expected Results** | 1. The component name updates to "Conference Room Sensor" on the canvas.<br>2. The name updates in Left Sidebar > Inventory.<br>3. No validation errors are shown. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.e - IWS - Rename component with special characters

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Open Right Sidebar > Properties drawer.<br>3. Attempt to rename the component to "IWS @#$%&*!" (special characters).<br>4. Click away to confirm. |
| **Expected Results** | 1. The component either accepts the name or displays a validation error if special characters are not permitted.<br>2. If accepted, the name displays correctly on the canvas and inventory. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.f - IWS - Add multiple IWS components

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design. |
| **Steps** | 1. Add a first IWS component to Center Workspace > Canvas.<br>2. Add a second IWS component to the canvas.<br>3. Add a third IWS component to the canvas. |
| **Expected Results** | 1. Each component gets a unique default name (e.g., "IWS 1", "IWS 2", "IWS 3").<br>2. All three components are listed in Left Sidebar > Inventory.<br>3. Each component can be independently selected and configured. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.g - IWS - Delete component from design

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Press the Delete key (or right-click and select "Delete").<br>3. Confirm deletion if prompted. |
| **Expected Results** | 1. The IWS component is removed from the canvas.<br>2. The component is removed from Left Sidebar > Inventory.<br>3. No orphaned references remain in the design. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.h - IWS - Double-click to open component window

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas. |
| **Steps** | 1. Double-click the IWS component on Center Workspace > Canvas. |
| **Expected Results** | 1. Floating Window "Intelligent Workspace Sensor" opens.<br>2. The window title bar reads "Intelligent Workspace Sensor".<br>3. Three tabs are visible: "Status", "LED Configuration", "Occupancy Sensor Configuration".<br>4. The "Status" tab is selected by default, showing sections: Status (with ID button), CPU Temp./Mobo Temp., Network, Sensor Output, Timeout Settings, and Group.<br>5. The window can be moved, resized, and closed. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.i - IWS - Verify no license required

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design with no additional licenses applied. |
| **Steps** | 1. Add an IWS component to Center Workspace > Canvas.<br>2. Review for any license warning or restriction messages.<br>3. Open Right Sidebar > Properties drawer and review all properties. |
| **Expected Results** | 1. The IWS component is added without any license warning.<br>2. All component features are accessible without additional license.<br>3. No "license required" indicators appear anywhere in the UI. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.j - IWS - Verify Sensor Group configuration

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, locate the Group section.<br>3. Enter a value in the "Sensor Group" field (e.g., "Building A - Floor 2").<br>4. Click away to confirm. |
| **Expected Results** | 1. The Sensor Group field accepts the entered value.<br>2. The value is displayed in the Group section.<br>3. The Sensor Group value can be used to logically group multiple IWS devices. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.k - IWS - Verify Timeout setting in minutes

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, locate the Timeout Settings section.<br>3. Enter a value in the "Timeout (mins)" field (e.g., 5).<br>4. Observe the Occupancy State behavior after people leave the sensor field of view. |
| **Expected Results** | 1. The Timeout field accepts the entered value in minutes.<br>2. After the last person leaves the field of view, the Occupancy State remains true/occupied for approximately the configured timeout duration.<br>3. After the timeout expires, Occupancy State changes to false/unoccupied. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.l - IWS - Verify Poll Rate setting in seconds

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, locate the Timeout Settings section.<br>3. Enter a value in the "Poll Rate (secs)" field (e.g., 2).<br>4. Observe the sensor data update frequency in the Sensor Output section. |
| **Expected Results** | 1. The Poll Rate field accepts the entered value in seconds.<br>2. Sensor data updates at approximately the configured interval.<br>3. Changing the poll rate visibly affects the update frequency. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.m - IWS - Verify Status tab Network section displays device info

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, review the Network section fields: Hostname, Model ID, System Uptime, Kernel Ver., Framework Ver. |
| **Expected Results** | 1. Hostname displays the device hostname.<br>2. Model ID displays the IWS model identifier.<br>3. System Uptime displays a time value.<br>4. Kernel Ver. displays a version string.<br>5. Framework Ver. displays a version string.<br>6. All values are populated and plausible. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.n - IWS - Verify ID button triggers device identification

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, locate the "ID" button in the Status section.<br>3. Click the "ID" button.<br>4. Observe the physical IWS device. |
| **Expected Results** | 1. The physical IWS device performs an identification action (e.g., LED ring flashes a distinct pattern).<br>2. The identification action is clearly visible and distinguishable from normal LED operation.<br>3. The identification stops after a period or when the button is toggled off. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.o - IWS - Verify CPU Temp and Mobo Temp display

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. On the Status tab, locate "CPU Temp." and "Mobo Temp." fields.<br>3. Observe the displayed values. |
| **Expected Results** | 1. CPU Temp. displays a numeric temperature value.<br>2. Mobo Temp. displays a numeric temperature value.<br>3. Both values are within plausible hardware temperature ranges.<br>4. Values update periodically. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.p - IWS - Verify Bluetooth is not available

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Review all tabs: Status, LED Configuration, Occupancy Sensor Configuration.<br>3. Inspect Right Sidebar > Properties drawer for any Bluetooth-related settings.<br>4. Review the control pins list for any Bluetooth-related pins. |
| **Expected Results** | 1. No Bluetooth configuration options are present in any tab.<br>2. No Bluetooth-related properties appear in the Properties drawer.<br>3. No Bluetooth-related control pins are exposed.<br>4. The device does not advertise or expose Bluetooth functionality in Q-SYS Designer. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |

---

## 01.q - IWS - Verify status indicator shows Fault when device is not connected

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. No IWS device is physically connected or commissioned to the system. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "Status" tab.<br>3. Observe the status indicator bar (located between the tab strip and the CPU Temp / Mobo Temp fields). |
| **Expected Results** | 1. The status indicator bar is **red**.<br>2. The status indicator displays the text "Fault".<br>3. The indicator clearly communicates that the device is not connected to the system. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > Component Basics |
