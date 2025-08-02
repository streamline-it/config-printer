# config_printer
Setup Printing for RHEL and FreeBSD hosts
# contents of defaults/main

# printer declaration variable
# Currently I am only supporting ipv4
config_printer_printers:
  - printer_name: 
    driver_filepath:
    printer_path:

# The following variables are used for the defaults/RedHat and defaults/FreeBSD files
# The values will be different based on OS specifics

# path and name to the config file
config_printer_config_file_path: 

# contents of RedHat_variables.yml under vars

# packages to install
config_printer_pkgs:
  - name:

# name of the printer service
config_printer_printer_svc:
