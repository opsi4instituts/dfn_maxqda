The initial version of this package was created by Eric Esser, Wissenschaftszentrum Berlin für Sozialforschung (Berlin Social Science Center) and published at the DFN-Repository of the initiative OPSI4instituts: https://opsi.wzb.eu
Contact, questions and suggestions: eric.esser@wzb.eu / opsi@wzb.eu

HOWTO
-----
1. Install the package on the OPSI server on the command line by "opsi-package-manager -i -p ask dfn_maxqda_<Versions-/Paketnummer>.opsi".
2. After the installation copy your Config.ini file with the licence information in the "custom" directory in the project folder of the product on the OPSI server and set the property kind-of-license to ini-file-in-custom-folder. Alternatively, set the property kind-of-license to opsi-property and enter the license name and the server name in the properties of the configed of OPSI. You can also hold the license name in a license pool of OPSI, but you still need to provide the server name in the opsi property.


PROPERTIES
----------
* desktopicon: Generate or delete desktop icon.
* custom-post-install: Define filename for include script in custom directory after installation.
* custom-post-deinstall: Define filename for include script in custom directory after deinstallation.
* remove-old-versions: Remove earlier installed versions of MAXQDA on this machine. Caution, this might remove a licensed older version and in order to retrieve the licence you have to contact MAXQDA support.
* kind-of-license: Defines the kind of license: "opsi-property" takes the license name from the property "licensename", "licensepool" uses the license name delivered by the license module of OPSI. The delivering license pool can be specified in the property "licensepoolname". "ini-file-in-custom-folder" uses the Config.ini file placed in the custom folder of the package and "testversion" installs MAXQDA as test version.
* licensename: The license name for your MAXQDA installation. Only needed if the property "kind-of-license" is set to "licensename".
* licensepoolname: The license pool name for OPSI license module. Only needed if the property "kind-of-license" is set to "licensepool".
* licenseserver: The fqdn or the IP of the license server or the IP of it. Only needed if the property "kind-of-license" is set to "opsi-property" or "licensepool".

