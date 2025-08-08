# the killer

In order to adapt to the new changes in nvgt0.90.0 dev, the following adjustments have been made.

*1. Change the bool using in the player class of * * player. nvgt * * on the server side; Variable, temporarily changed to bool using1 due to conflict with nvgt;

* 2. Due to changes in the functions of the 3D audio system, the switch for the 3D audio system has been rewritten.

* 3. Currently, the default pack_defiles class does not have a list_defile method. If you want to list files, you need to write: cast<pack_file@>(sound_default_pack).list_files();

* 4. A new package creator has been created to create the latest package files, which can be encrypted. The previous package creator is not available in the latest version of nvgt.
