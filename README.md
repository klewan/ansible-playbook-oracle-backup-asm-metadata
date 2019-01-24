Ansible Playbook: oracle-backup-asm-metadata
============================================

This playbook performs ASM metadata backup including OCR/OLR ocrconfig manualbackup and export OCR/OLR contents and ASM meetadata to a file.

Supported OS:
-------------
* RedHat
* CentOS
* OracleLinux

Requirements
------------

This playbook requires the `oracle` and `oracle-asm-metadata` roles.

`$ ansible-galaxy install -r roles/requirements.yml`

Examples
--------

    $ ansible-playbook playbook.yml --list-tasks
    $ ansible-playbook playbook.yml --list-tags

Default execution:

    ansible-playbook playbook.yml

Perform backup ASM metadata without RAC support:

    ansible-playbook playbook.yml --extra-vars='{"_oracle_backup_asm_metadata_rac_support": false}'

	
License
-------

GPLv3 - GNU General Public License v3.0

Author Information
------------------

This playbook was created in 2018 by [Krzysztof Lewandowski](mailto:Krzysztof.Lewandowski@fastmail.fm).

