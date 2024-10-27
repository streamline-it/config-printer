# printer_config
Setup Printing for RHEL and FreeBSD hosts
# contents of defaults/main

# printer declaration variable
# Currently I am only supporting ipv4
printer_config_printers:
  - printer_name: 
    printer_ipv4:
    printer_ipv6:

# The following variables are used for the defaults/RedHat and defaults/FreeBSD files
# The values will be different based on OS specifics

# path and name to the config file
printer_config_config_file_path: 

# contents of RedHat_variables.yml under vars

# packages to install
printer_config_pkgs:
  - name:

# name of the printer service
printer_config_printer_svc:
