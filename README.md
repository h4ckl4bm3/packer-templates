# Packer Templates

This is a set of templates designed for use with Packer to make VMware and VirtualBox images for PuPHPet boxes.

It can be used to generate custom boxes not provisioned by PuPHPet, though!

# Instructions

    $ git clone https://github.com/puphpet/packer-templates
    $ cd packer-templates
    $ packer build template.json

If you want to build only virtualbox or vmware.

    $ packer build -only=virtualbox-iso template.json
    $ packer build -only=vmware-iso template.json
    $ packer build -only=parallels-iso template.json

VMWare requires VMware OVF Tool installed. Simply create a VM using VMWare GUI.

Parallel builds can be run on 0.6.0 or latest packer version and requires Parallels Virtualization SDK installed.

# Credit

Shamelessly stolen from https://github.com/smerrill/packer-templates and customized
by Juan Treminio to fit into PuPHPet's workflow
