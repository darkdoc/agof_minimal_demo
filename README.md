# Ansible GitOps Framework Minimal Project Demo

## What is this?

This is a minimalistic AAP project that is used in the demonstration of how to use AGOF, an Ansible GitOps Framework.

This project contains a playbook and inventory, which AGOF will load into Ansible Automation Platform, and runs the template as a job. The entire pattern depends only on the AAP controller, and the template job connects to, elevates privileges on, and gathers facts from the AAP node.

The intention is to provide an example to build on, to build more interesting patterns with.

## How do I get started?

1. Check out the AGOF [repository](https://github.com/validatedpatterns/agof), which will serve as the provisioner for the pattern
1. Configure an `~/agof_vault.yml` file with your AWS credentials and configuration
1. Run `./patterns.sh make intall` from the AGOF repository directory. If you are using the [minimal config repository](https://github.com/validatedpatterns-demos/agof_minimal_config) it will include this repository as its project.
