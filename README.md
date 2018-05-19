# Hammer via Docker

Execute commands for administrative tasks on an **external** Foreman or Smart Proxy servers via a Docker instance.

## Usage (abbreviated output)

    $ docker run -t hammer:latest -s https://<SERVER>
    Usage:
        hammer [OPTIONS] SUBCOMMAND [ARG] ...
    
    Parameters:
     SUBCOMMAND                    Subcommand
     [ARG] ...                     Subcommand arguments

    Subcommands:
     admin                         Administrative server-side tasks
     architecture                  Manipulate architectures
     auth                          Foreman connection login/logout
     auth-source                   Manipulate auth sources
     compute-resource              Manipulate compute resources
     config-group                  Manipulate config groups
     defaults                      Defaults management

    $ docker run -t hammer:latest -s https://<SERVER> organization list
    ---|----------------------|----------------------|----------------------------
    ID | TITLE                | NAME                 | DESCRIPTION
    ---|----------------------|----------------------|----------------------------
    1  | Default Organization | Default Organization |
    3  | São Paulo            | São Paulo            | The São Paulo organization.
    ---|----------------------|----------------------|----------------------------
