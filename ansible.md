missing-become-password

ref: https://discourse.roots.io/t/reprovision-suddenly-gives-missing-become-password-error/4584

Awesome you've added that security. Check out the Security wiki19 which mentions how you'll need to add the --ask-become-pass flag to your ansible-playbook command now that root login is disabled. So, try this:
ansible-playbook server.yml -i hosts/staging --ask-become-pass

Or use -K (that's a capital K) for short:
ansible-playbook server.yml -i hosts/staging -K
