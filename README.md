
# ansible-apply-role

Sometimes, you don't want to write a playbook to run a role against a machine.
I find this is true when I'm on a machine and want to add another role to it so
that I can work on a new project.

This tool assumes that any role you want to run is accessible to 
`ansible-playbook`

e.g. If I wanted to install NodeJS on my current machine to work on a project, I
could run:

```bash
ansible-apply-role geerlingguy.nodejs
```

This will run the `geerlingguy.nodejs` role with all the default variables. If
you want to customise the install, I'd recommend using your own custom role that
sets all the required variables.
