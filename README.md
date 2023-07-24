# Ansible GitOps Framework Minimal Demo

## What is this?

This is a minimalistic pattern that demonstrates how to use AGOF, an Ansible GitOps Framework.

It contains configuration suitable to load a project, inventory, and template into Ansible Automation Platform, and runs the template as a job. The entire pattern depends only on the AAP controller, and the template job connects to, elevates privileges on, and gathers facts from the AAP node.

The intention is to provide an example to build on, to build more interesting patterns with.

## How do I get started?

1. Check this repository out
1. Check out the AGOF [repostitory](https://github.com/hybrid-cloud-patterns/agof), which will serve as the provisioner for the pattern
1. Configure an `~/agof_vault.yml` file with your AWS credentials and configuration
1. Run `./patterns.sh make intall` from the AGOF repository directory, with `controller_config_dir` set to this repository's `config` directory. If this repo is checked out as `~/gitwork/agof_minimal_demo`, the setting should look like: `controller_config_dir: '{{ '~/gitwork/agof_minimal_demo/config' | expanduser }}`.
