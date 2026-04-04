​Project: Mobile OS Hardening & Privacy Audit
​1. Objective
​The goal of this audit was to identify and disable "Observer" services and "Telemetry" (data tracking) on a mobile device to reduce the attack surface and increase user privacy.
​2. Audit Findings
​Service Analysis (Ad Privacy): Identified the Ad Privacy process running in the system services. While this service acts as a mediator for the "Privacy Sandbox," it still functions as a local observer of user interests.
​Vulnerability Assessment (Debug Logging): Discovered the Enable debug logging for ads toggle was available.
​3. Security Actions Taken
​Hardening: Explicitly verified that Debug Logging is OFF.
​Risk Mitigation: By keeping debug logging disabled, I am preventing the system from writing sensitive network traffic data and device identifiers to the System Log, which could be exploited by malicious applications.
​Privacy Control: Managed "Ad Topics" to limit the profile the internet machine builds based on my app usage.
​4. Conclusion
​A "Security-First" mindset requires constant auditing of running services. By disabling non-essential debugging and restricting tracking IDs, I have successfully hardened the device against passive data collection
