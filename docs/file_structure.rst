File structure
==============

The IP HDK contains the components and models for compilation and simulation of the assembly IP core + IP Activator.

IP Activator HDK directories and files:

.. code-block:: bash

   drm_ip_activator_hdk_x.y.z/
   -- rtl/
   ---- altera/
         drm_all_components.vhdl
   ---- xilinx/
   -------- drm_all_components.vhdl
   -------- drm_ip_activator_0xvvvvllllnnnnvvvv.vhdl
   -------- drm_ip_activator_0xvvvvllllnnnnvvvv.vho
   -------- drm_ip_activator_0xvvvvllllnnnnvvvv.veo
   -------- drm_ip_activator_0xvvvvllllnnnnvvvv.v
   -------- drm_ip_activator_0xvvvvllllnnnnvvvv.xml
   -------- drm_activation_code_package_0xvvvvllllnnnnvvvv.vhdl
   -------- drm_activation_code_package_0xvvvvllllnnnnvvvv.v
   -- simu/
   ---- modelsim/
   -------- drm_all_components.vhdl
   -------- drm_controller_bfm.vhdl
   -------- drm_controller_bfm.v
   -------- drm_license_package.vhdl
   -- docs/



The archive file name postfix x.y.z is  the version number of the HDK.

For example "2.1.1.". **This version number must be specified when asking for a License File**.

The IP Activator entity name is DRM_IP_ACTIVATOR_0xVVVVLLLLNNNNVVVV with the postfix being a 64 bits hexadecimal encoding of the IP VLNV.

For example DRM_IP_ACTIVATOR_0x0C001020A56E0001
