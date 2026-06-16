# freeswitch-repo
freeswitch integration and deployment on a data center deployed on prem server , Debian based freeswitch 

# Custom FreeSWITCH Deployment Showcase

## System Specifications
* **Host OS:** Debian GNU/Linux 12 (bookworm) x86_64
* **FreeSWITCH Core:** Version 1.11.1-release (64bit)
* **Status:** Fully functional SIP registrar and media routing engine

## Testing & Verification
This setup was successfully verified using the following loopback route:
1. Connected a SIP softphone to the internal profile.
2. Dialed the global echo extension **9196**.
3. Confirmed proper audio stream negotiation (RTP) and zero-loss playback.

### Multi-User Call Verification
* **Extension 1000**: Provisioned and registered via SIP softphone.
* **Extension 1001**: Provisioned and registered via secondary endpoint.
* **Result**: Confirmed successful dialing from 1000 -> 1001 with clean bridge execution and active bidirectional audio streaming.

