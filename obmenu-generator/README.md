# Mi configuración de obmenu-generator


**Configuración:**

$ obmenu-generator -h
usage: /usr/bin/obmenu-generator [options]

menu:
    -p         : generate a dynamic menu (pipe)
    -s         : generate a static menu
    -i         : include icons
    -m <id>    : menu id (default: 'root-menu')
    -t <label> : menu label text (default: 'Applications')

other:
    -S <file>  : path to the schema.pl file
    -C <file>  : path to the config.pl file
    -o <file>  : path to the menu.xml file
    -u         : update the config file
    -r         : regenerate the config file
    -d         : regenerate icons.db
    -c         : reconfigure openbox automatically
    -R         : reconfigure openbox and exit
    -h         : print this message and exit
    -v         : print version and exit

examples:
        /usr/bin/obmenu-generator -p -i     # dynamic menu with icons
        /usr/bin/obmenu-generator -s -c     # static menu without icons

=> Config file: /home/ice/.config/obmenu-generator/config.pl
=> Schema file: /home/ice/.config/obmenu-generator/schema.pl


**Importante:** Tengan en cuenta que se ve la configuración de mi home, cuando ejecuten la sentencia, les aparecerá su home.


**Mi configuración:**
obmenu-generator -p -c 

- Agregué en la categoría Exit, aparte la clásica de Exit (para salir de Openbox), dos más que son Reboot y Shutdown, que ya saben para que son.
- Comenté el ítem de gmrun ya que no lo uso.
- En config.pl modifique el editor a Sublime-Text-3 que es mi preferido en las X y para la tty uso nano.

Quedando como resultado:

![texto cualquiera por si no carga la imagen](http://i.imgur.com/rhKVMCU.png)
