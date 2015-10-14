#Broken relative paths in ansible

Doing some imports and it works in older versions of Ansible.

Current version:

    ansible 2.0.0 (devel 8277747a04) last updated 2015/10/12 21:06:26 (GMT-600)
      lib/ansible/modules/core: (detached HEAD 92d25017ed) last updated
      2015/10/12 13:31:58 (GMT -600)
      lib/ansible/modules/extras: (detached HEAD 205115ea1f) last updated
      2015/10/12 13:32:08 (GMT -600)
      config file = /Users/derekcarter/.ansible.cfg
      configured module search path = None

To see what I mean run this:

    ansible-playbook -i hosts working.yml

And compare to this:

    ansible-playbook -i hosts broken.yml

