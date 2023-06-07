# Brief Introduction

To solve the problem of service abnormal OOM, the OOM generated by sudden memory growth cann't be quickly located.
The purpose of this service is to help users automatically locate the OOM problem and provide the corresponding OOM analysis report.

# Module Introduction
- **Monitor Module**: Memory changes are detected every second
- **Forward Module**: The memory change data is sent to the server
  - Support Webhook

# TODO

## v0.0.5
- [x] Support trigger indicator hot loading
  - use `Apply` to reload the trigger indicator
- [x] Provide default trigger indicator
  - if cooling time is 0, use the default cooling time [1m]
  - if memory absolute value is 0, use the default value [128Mib]
  - if diff is 0, use the default diff [10%]
