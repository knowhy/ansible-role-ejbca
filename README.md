# Ansible Role: EJBCA

Installs and configures EJBCA with JBOSS and MariaDB on RHEL7/CentOS7 servers.

Currently this is a shitty role. I publish this role because installation of EJBCA was always a pain for me and I hope that this role might make your life a bit easier.

The role install [JBoss Application Server 7](https://jboss.org/jbossas "JBoss AS Homepage") and [EJBCA](https://www.ejbca.org "EJBCA Homepage").

## Requirements

None

## Role Variables

## EJBCA usage

run the play. The play will install JBOSS 7.1.1, MariaDB and EJBCA. EJBCA is installed via ant during the play.

## RHEL/CentOS 7 EJBCA configuration

Set the following variables (at a minimum):

    ejbca_mysql_password

** TODO define variables

## Example Playbook

    - hosts: pki-servers
      vars_files:
        - vars/main.yml
      roles:
        - { role: knowhy.ejbca }

## License

MIT / BSD

## Author Information

This role was created in 2015 by Henrik Pingel.