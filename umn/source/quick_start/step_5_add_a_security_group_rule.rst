:original_name: qsg_0007.html

.. _qsg_0007:

Step 5: Add a Security Group Rule
=================================

Scenarios
---------

After you create a security group, you can add rules to the security group. A rule applies either to inbound traffic or outbound traffic. After you add cloud resources to the security group, they are protected by the rules of the group.

-  Inbound rules control incoming traffic to cloud resources in the security group.
-  Outbound rules control outgoing traffic from cloud resources in the security group.

Procedure
---------

#. Log in to the management console.

#. Click |image1| in the upper left corner and select the desired region and project.

#. On the console homepage, under **Network**, click **Virtual Private Cloud**.

#. In the navigation pane on the left, choose **Access Control** > **Security Groups**.

#. On the **Security Groups** page, locate the target security group and click **Manage Rule** in the **Operation** column to switch to the page for managing inbound and outbound rules.

#. On the **Inbound Rules** tab, click **Add Rule**. In the displayed dialog box, set required parameters.

   You can click **+** to add more inbound rules.

   .. table:: **Table 1** Inbound rule parameter description

      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                                                                                                                                          | Example Value         |
      +=======================+======================================================================================================================================================================================+=======================+
      | Protocol & Port       | **Protocol**: The network protocol. Currently, the value can be **All**, **TCP**, **UDP**, **ICMP**, **GRE**, or others.                                                             | Custom TC             |
      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      |                       | **Port**: The port or port range over which the traffic can reach your ECS. The value ranges from 1 to 65535.                                                                        | 22, or 22-30          |
      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Source                | The source of the security group rule. The value can be a single IP address or a security group to allow access from the IP address or instances in the security group. For example: | 0.0.0.0/0             |
      |                       |                                                                                                                                                                                      |                       |
      |                       | -  Single IP address: 192.168.10.10/32 (IPv4); 2002:50::44/127 (IPv6)                                                                                                                |                       |
      |                       | -  IP address range: 192.168.1.0/24 (IPv4); 2407:c080:802:469::/64 (IPv6)                                                                                                            |                       |
      |                       | -  All IP addresses: 0.0.0.0/0 (IPv4); ::/0 (IPv6)                                                                                                                                   |                       |
      |                       | -  Security group: sg-abc                                                                                                                                                            |                       |
      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Description           | Supplementary information about the security group rule. This parameter is optional.                                                                                                 | ``-``                 |
      |                       |                                                                                                                                                                                      |                       |
      |                       | The security group rule description can contain a maximum of 255 characters and cannot contain angle brackets (< or >).                                                              |                       |
      +-----------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. On the **Outbound Rules** tab, click **Add Rule**. In the displayed dialog box, set required parameters.

   You can click **+** to add more outbound rules.

   .. table:: **Table 2** Outbound rule parameter description

      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Parameter             | Description                                                                                                                                                                             | Example Value         |
      +=======================+=========================================================================================================================================================================================+=======================+
      | Protocol & Port       | **Protocol**: The network protocol. Currently, the value can be **All**, **TCP**, **UDP**, **ICMP**, **GRE**, or others.                                                                | Custom TCP            |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      |                       | **Port**: The port or port range over which the traffic can leave your ECS. The value ranges from 1 to 65535.                                                                           | 22, or 22-30          |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Destination           | The destination of the security group rule. The value can be a single IP address or a security group to allow access to the IP address or instances in the security group. For example: | 0.0.0.0/0             |
      |                       |                                                                                                                                                                                         |                       |
      |                       | -  Single IP address: 192.168.10.10/32 (IPv4); 2002:50::44/127 (IPv6)                                                                                                                   |                       |
      |                       | -  IP address range: 192.168.1.0/24 (IPv4); 2407:c080:802:469::/64 (IPv6)                                                                                                               |                       |
      |                       | -  All IP addresses: 0.0.0.0/0 (IPv4); ::/0 (IPv6)                                                                                                                                      |                       |
      |                       | -  Security group: sg-abc                                                                                                                                                               |                       |
      |                       |                                                                                                                                                                                         |                       |
      |                       | For more information, see *Virtual Private Cloud User Guide*.                                                                                                                           |                       |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+
      | Description           | Supplementary information about the security group rule. This parameter is optional.                                                                                                    | ``-``                 |
      |                       |                                                                                                                                                                                         |                       |
      |                       | The security group rule description can contain a maximum of 255 characters and cannot contain angle brackets (< or >).                                                                 |                       |
      +-----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------------+

#. Click **OK**.

.. |image1| image:: /_static/images/en-us_image_0141273034.png
