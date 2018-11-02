Operations
==========

All signals of the IP Core I/F are synchronized with the IP Core clock domain (internal CDC with the DRM Clock domain in the IP Activator).

The IP Core captures the Activation Code when the Activation Code Ready output is '1'.

The IP Core uses the 128 bits of the Activation Code output to control its features enabling.

An internal Credit Timer is used for Demo License or Simulation License: its initialization is done by the DRM IPs with the value provided in the license file and its decrement is under the control of the IP Core by setting the input DRM_EVENT to '1'. The IP Core knows that a temporary Activation Code has been loaded in the IP Activator when the DEMO_MODE output is set to '1'. The IP Core detects the Activation timeout when the Activation Code Ready output is '0' and/or the Activation Code output is all 0’s.

An internal Metering counter is used to store the activity of the IP Core: it is asynchronously reset upon the IP_CORE_aRSTn input and is synchronously reset by the DRM Controller via the DRM Bus; its increment is under the control of the IP Core by setting the input DRM_EVENT to '1'.