:original_name: eip_0021.html

.. _eip_0021:

Supported EIP Operations
========================

With CTS, you can record operations performed on the VPC service for further query, audit, and backtracking purposes.

:ref:`Table 1 <eip_0021__en-us_topic_0118498910_table19292448162913>` lists the EIP operations that can be recorded by CTS.

.. _eip_0021__en-us_topic_0118498910_table19292448162913:

.. table:: **Table 1** EIP operations that can be recorded by CTS

   ============================== ============= ===============
   Operation                      Resource Type Trace
   ============================== ============= ===============
   Modifying a bandwidth          bandwidth     modifyBandwidth
   Assigning an EIP               eip           createEip
   Releasing an EIP               eip           deleteEip
   Binding an EIP                 eip           bindEip
   Unbinding an EIP               eip           unbindEip
   Assigning a private IP address privateIps    createPrivateIp
   Releasing a private IP address privateIps    deletePrivateIp
   ============================== ============= ===============
