# KAMATERA SCRIPTS

A collection of command line programs for managing servers
with [kamatera](https://go.kamatera.com) cloud provider.

This script's use 'curl' and 'jq' for making the REST requests.

They have been tested with dash, bash, ash (busybox) in march
of 2023.

## Configuration.

Only two environment variables are necessary. You can get them
in the kamatera console.

- KAMATERA_API_CLIENT_ID
- KAMATERA_API_SECRET

## Help

kamatera-h-billing

    Usage: kamatera-h-billing [-m MONTH] [-y YEAR]
    
    Fetch billing information for the month.

kamatera-h-create

    Usage: kamatera-h-create [OPTIONS...]
    
    Create a new server in Kamatera Cloud.
    
        -V         : Show configuration.
        -P s|l     : Set computing power.
        -n NAME    : Name for the new machine.
        -s SECRET  : Password for the new machine ($KAMATERA_PASSWORD).
        -i IMAGE|l : Specify an image.
    

kamatera-h-create-options

    Usage: kamatera-h-create-options [OPTS...]
    
    Download the creation options for kamatera-h-create(1) to
    cache and show.
    
        -l : List images.

kamatera-h-info

    Usage: kamatera-h-info NAME|UUID
    
    Fetch server information.

kamatera-h-ipaddr

    Usage: kamatera-h-ipaddr UUID|NAME
    
    Get server's first IP address.

kamatera-h-ls

    Usage: kamatera-h-ls
    
    List servers. (ID, DATACENTER, NAME, POWER).

kamatera-h-ls-hosts

    Usage: kamatera-h-ls-hosts
    
    Print server's names and IP addresses in /etc/hosts format.

kamatera-h-passwd

    Usage: kamatera-h-passwd MACHINE
    
    Change the password to $KAMATERA_PASSWORD to the root user in
    the specified machine.
    

kamatera-h-power

    Usage: kamatera-h-power OPTS... MACHINE
    
    Check or change the power status of a machine.
    
       -p : Power off machine.
       -r : Restart machine.
       -s : Start machine.
       -c : Print "on" or "off".
    

kamatera-h-queue

    Usage: kamatera-h-queue : View the task queue.

kamatera-h-rename

    Usage: kamatera-h-rename [FROM [TO]]
    
    Rename a server's name.

kamatera-h-rest

    Usage: kamatera-h-rest -V | [-q] PATH

kamatera-h-ssh

    Usage: kamatera-h-ssh [OPTS...] MACHINE|UUID
    
       -i : Install public keys.
       -c : Print SSH configuration.

kamatera-h-uuid

    Usage: kamatera-h-uuid NAME
    
    The the UUID of a server.

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
