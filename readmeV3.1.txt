README.TXT
++++++++++
Installing Actuate BIRT iHub System, Actuate BIRT iHub Personal Development Edition and Actuate Java Components key files
============================================================================================================================

Actuate provides license key files to use when installing Actuate BIRT iHub System and Actuate Java Components products.  The following e-mail describes the process for installing these license key files.

Obtaining a license key file
----------------------------

To obtain a new license key file for a licensed product or receive assistance with a license key already issued to you, visit the e.Support web site at: http://support.actuate.com. Choose the dropdown for Support Online->License Keys. A maintenance customer should have login information for the Actuate e.Support web site. If you do not have access, please contact Actuate Support at support@actuate.com. You can also contact Actuate Customer Care at customercare@actuate.com. 

Installing the Actuate BIRT iHub System license file (if you are using the Personal Development Edition, please scroll down to the appropriate section below)
-------------------------------------------------------------------------------------------------------------------------------------------------------------
New customers receive this e-mail containing the license key files after Actuate processes the order. Actuate BIRT iHub System customers, who require node-key licenses, perform an initial installation. After installing Actuate BIRT iHub System, the installation informs a customer requiring a node-key license to obtain the machine ID information on which Actuate BIRT iHub is running and transmit this information to Actuate Licensing. The machine ID is displayed in the reminder message. You can also use the utility, acmachineid, to obtain the machine ID. For information on how to use the acmachineid utility, see the instructions in this message.

After receiving the machine ID information, Actuate Licensing will issue a new Actuate BIRT iHub System key file and transmit it to you attached to this message.

If you receive this e-mail after performing an installation of Actuate BIRT iHub System and transmitting the required machine ID information to obtain a node-key license, this ZIP file contains the following files:

- readme.txt
  The text of this e-mail

- Actuate_iHub_key_XXXXXXX.xml
  Actuate BIRT iHub System key license.  


To update the license key file, perform the following steps:
1.  Copy the Actuate_iHub_key_XXXXXXX.xml license file to the location specified by the AC_CONFIG_HOME variable in the <AC_SERVER_HOME>\etc\acpmdconfig.xml file and rename the Actuate_iHub_key_XXXXXXX.xml file to acserverlicense.xml.  Replace any previous acserverlicense.xml file.
2.  To take into effect with the new license key, restart ihub3.1 on all the node(s).


How to use the acmachineid utility
----------------------------------
You can use the acmachineid utility to obtain the machine ID information as shown in the following command-line example:

C:\Program Files\Actuate\iHub3\bin>acmachineid

STATUS:         OK
GEN_VERSION:    23 iHub
GEN_BUILD:      220A130129
MACHINEID:      q0RREHs0Jk6tu0o8AbCrVL61x4kDpLlQKwS2t1W7qM6LGbO8VjcFs6pcuAgbtDa/ZauSbFFa2mRejwVJc7ZjKfMEVl1suXglMKmZLiwtLykwJisqMS0EhY+5sCYoKjG+XIWsEnL2GGhLtI9fJUMYzCEKW7yujw0DgE6rogKsvlc

The acmachineid utility is located in <iHub home directory>/bin. 

Send Actuate licensing the output of the machineid utility.

*** NODE LOCK FILES ***
If you change the machine on which you installed Actuate BIRT iHub, you must re-apply to Actuate Licensing for a new license file. If you replace the network card on some machines, such as a Windows system, you may have to obtain a new license key file since the unique identifier for the network card may be the source of the machine ID. If you have a license file installed and a reminder message appears when logging into Actuate Management Console, contact Actuate Licensing and provide the current Actuate iHub System license file with the output from the machine ID utility.

Note: The Actuate_iHub_key_XXXXXXX.xml will contain the node key information for the standalone machine or all machines in a cluster.  There is no separate node license key file for each machine.

*** MODIFIED LICENSES ***
If you decide later to license additional iHub options, the existing set of license files becomes invalid. You must install new Actuate BIRT iHub System and node-key files.


Installing the Actuate BIRT iHub Personal Development Edition license file
--------------------------------------------------------------------------    
New customers receive this e-mail containing the license key files after Actuate processes the order. After installing Actuate BIRT iHub Personal Development Edition System, customer will need to register and apply Activation Code by accessing the BIRT iHub Visualization Console (Default url: http://<hostname>:8700/iportal). 


The ZIP file attached to this email contains the following files:

- readme.txt
  The text of this e-mail

- Actuate_iHub_key_XXXXXXX.xml
  Actuate BIRT iHub System key license.  


To update the license key file, perform the following steps:

1. Copy the Actuate_iHub_key_XXXXXXX.xml license file to the AC_CONFIG_HOME. (If you are unsure of the location, AC_CONFIG_HOME is defined in the <AC_SERVER_HOME>/etc/acpmdconfig.xml file.)
2. Rename the Actuate_iHub_key_XXXXXXX.xml file to acserverlicense.xml. Replace any previous acserverlicense.xml file.
3. To take into effect with the new license key, restart ihub3.1.

*** MODIFIED LICENSES ***
If you decide later to license additional iHub options, the existing set of license files becomes invalid. You must install new Actuate BIRT iHub System license.


How to install an Actuate Java Component license key file
---------------------------------------------------------
1. Extract the Actuate Java Component War/Ear file.
2. Replace the ajclicense.xml file located in the <War file root>/WEB-INF directory with the new Actuate Java Component license file received. Make sure to rename the file received to ajclicense.xml.
3. Rebuild the War/Ear file with the new license file.
4. Redeploy the War/Ear and restart the application.
