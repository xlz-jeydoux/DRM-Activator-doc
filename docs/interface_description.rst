Interface description
=====================

The communication on the DRM Bus uses a proprietary protocol where the IP Activator is a slave, the DRM Controller being the master.

**DRM Bus Socket connected to DRM controller**:

Proprietary protocol


**DRM Activator interface with IP to protect**:

The interface with the IP Core is a simple register interface with control signals.

.. list-table::
   :header-rows: 1

   * - Name
     - Direction
     - Size
     - Description
   * - IP_CORE_aCLK
     - in
     - 1
     - IP Core clock
   * - IP_CORE_aRSTn
     - in
     - 1
     - IP Core Asynchronous Reset (active low)
   * - DRM_EVENT
     - in
     - 1
     - Decrements the Credit timer and Increments the Metering counter when set to '1'; Synchronous with IP_CORE_aCLK
   * - ACTIVATION_CODE
     - out
     - 128
     - The Activation Code (synchronous to IP_CORE_aCLK)
   * - ACTIVATION_CODE_READY
     - out
     - 1
     - Tells that an Activation Code is available when set to '1'
   * - DEMO_MODE
     - out
     - 1
     - Tells that the Activation Code is temporary (synchronous to IP_CORE_aCLK)

    