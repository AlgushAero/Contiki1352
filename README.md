# Contiki1352

**Contiki1352** is NOT a fork of Contiki. It is an independent project with the primary goal of implementing a mesh network in the most effective and TI-centered way for CC1352 microchips.

## Comparison

| Contiki1352                      | Contiki-NG                                         |
|----------------------------------|----------------------------------------------------|
| Only for TI CC1352               | Supports dozens of microchips                      |
| 4MHz RAT timer (precision -> power saving) | 32kHz timer (wasting CPU time and radio time)  |
| Various proprietary protocols    | Strict to 802.15.4                                 |
| Pass-by-value `uint32_t`/`uint64_t` ID  | Pass-by-reference `linkaddr_t*`              |
| TI SDK libs                      | Custom lists, tables, queues, etc.                 |
| Multiple networks, multiple border devices | Operates only 1 network at a time             |
| Full BLE support (OtAD, various iOS/Android apps) | No BLE (BLE advertising only)     |

## Basic Rules

*(These can be reviewed if necessary)*

- Utilize CC1352 capabilities.
- Use CCStudio.
- Use ticlang.
- Use the TI SDK.
- Use SysConfig where possible (it helps new users).
- Please document step-by-step instructions on how to build/rebuild the system from the standard SDK.
