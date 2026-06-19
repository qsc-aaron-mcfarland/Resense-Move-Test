# Pending Clarifications

## 12.a - Factory Reset

- What happens to the device's relationship with the Core after factory reset?
- Does the device name revert so it no longer matches the inventory item?
- Does it need re-pairing, re-matching, or something else to reconnect?
- Preconditions still say "commissioned and connected" — update once behavior is confirmed
- Expected result #5 says "requires re-commissioning" — rewrite once clarified

## 16 - Web UI (New Section)

Reviewer feedback: the test plan omits most Web UI functionality. New section 16 needed.

### 16.1 - IR frame rendering & color remapping
- DRAFTED (16.a, 16.b, 16.c) — 4 palette options, auto-refresh, persistence on reload
- Red area = lens boundary (physical FOV edge), not an error state

### 16.2 - Installation icon show/hide
- Awaiting clarification on what the icon represents and toggle behavior

### 16.3 - Layout persistence for multi sensor
- DRAFTED (16.d) — spatial arrangement persists across a group

### 16.4 - Grouping logic
- DRAFTED (16.e, 16.f) — add/remove sensors, combined zone view
- Configured in Web UI only (not Designer)

### 16.5 - Error states for zones outside tracking area
- Per reviewer: currently does nothing when zone extends beyond lens boundary
- Need clarification: is this a planned feature (show warning/error) or acceptable behavior?
- Also pending: what is the "refresh" behavior testing scope?
