# LED Configuration Test Cases

## 03.a - IWS - Verify LED ring color control available

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED ring color control. |
| **Expected Results** | 1. LED ring color control is visible on the LED Configuration tab.<br>2. Color selection options are available (e.g., color picker, RGB values, or preset colors). |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.b - IWS - Set LED ring to a specific color

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Color control.<br>4. Set the LED color to red (R:255, G:0, B:0 or equivalent).<br>4. Observe the physical IWS device. |
| **Expected Results** | 1. The LED ring color value updates to red in the UI.<br>2. The physical IWS device LED ring illuminates red. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.c - IWS - Set LED ring brightness to maximum

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Brightness control.<br>4. Set brightness to maximum (100%). |
| **Expected Results** | 1. The brightness value shows 100% in the UI.<br>2. The physical IWS device LED ring is at maximum brightness. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.d - IWS - Set LED ring brightness to minimum

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Brightness control.<br>4. Set brightness to minimum (0%). |
| **Expected Results** | 1. The brightness value shows 0% in the UI.<br>2. The physical IWS device LED ring is off or at minimum brightness. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.e - IWS - Set LED ring brightness to midrange value

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Brightness control.<br>4. Set brightness to 50%.<br>5. Observe the physical IWS device. |
| **Expected Results** | 1. The brightness value shows 50% in the UI.<br>2. The physical IWS device LED ring brightness is noticeably dimmer than maximum but still illuminated. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.f - IWS - Turn LED ring off

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. The LED ring is currently illuminated. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Enable control.<br>4. Turn the LED ring off. |
| **Expected Results** | 1. The LED status in the UI shows off/disabled.<br>2. The physical IWS device LED ring turns off completely. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.g - IWS - Turn LED ring on after being off

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. The LED ring is currently off. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Enable control.<br>4. Turn the LED ring on. |
| **Expected Results** | 1. The LED status in the UI shows on/enabled.<br>2. The physical IWS device LED ring illuminates with the previously configured color and brightness. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.h - IWS - Cycle through multiple LED colors

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Set the LED color to red and observe.<br>3. Change the LED color to green and observe.<br>4. Change the LED color to blue and observe.<br>5. Change the LED color to white and observe. |
| **Expected Results** | 1. Each color change is reflected in the UI immediately.<br>2. The physical IWS device LED ring changes color to match each selection.<br>3. No color bleed or artifacts from previous colors remain. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.i - IWS - Verify LED control with device disconnected

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device was previously commissioned, then disconnected from network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Attempt to change the LED ring color.<br>3. Attempt to change the LED ring brightness. |
| **Expected Results** | 1. The UI allows modifying the LED values.<br>2. The component status indicates the device is disconnected.<br>3. No crash or unhandled error occurs when sending LED commands to a disconnected device. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.j - IWS - Verify LED settings via control pins

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Select the IWS component on Center Workspace > Canvas.<br>2. Verify LED-related control pins are exposed: "LED Color", "LED Brightness", "LED Enable", "LED Pattern", "LED Speed".<br>3. Connect a script or control component to the LED control pins.<br>4. Send values via the control pins to change color, brightness, pattern, and speed. |
| **Expected Results** | 1. All five LED-related control pins are available and exposed on the component.<br>2. Sending values via control pins changes the LED ring on the physical device.<br>3. The Floating Window "Intelligent Workspace Sensor" > LED Configuration tab reflects the updated LED values. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.k - IWS - Verify LED Pattern control

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network. |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Pattern control.<br>3. Cycle through available LED patterns.<br>4. Observe the physical IWS device for each pattern. |
| **Expected Results** | 1. Multiple LED patterns are available for selection.<br>2. Each pattern produces a visually distinct effect on the physical LED ring (e.g., solid, pulse, chase, breathe).<br>3. The selected pattern is reflected in the UI. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |

---

## 03.l - IWS - Verify LED Speed control

| Field | Details |
|---|---|
| **Preconditions** | 1. Open "Q-SYS Designer" software.<br>2. Create a new design.<br>3. Add an IWS component to the canvas.<br>4. IWS device is commissioned and connected on the network.<br>5. LED Pattern is set to an animated pattern (not solid). |
| **Steps** | 1. Double-click the IWS component to open Floating Window "Intelligent Workspace Sensor".<br>2. Select the "LED Configuration" tab.<br>3. Locate the LED Speed control.<br>3. Set the speed to a low value and observe the LED animation.<br>4. Set the speed to a high value and observe the LED animation. |
| **Expected Results** | 1. The LED animation speed on the physical device changes with each setting.<br>2. The speed change is visually noticeable.<br>3. The speed value is reflected in the UI. |
| **Execution Type** | Manual |
| **Section** | Designer > Components > IWS > LED Configuration |
