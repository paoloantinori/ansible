% title: Ansible
% subtitle: The good, the bad, but mostly the ok parts
% author: Paolo Antinori
% author: Software Engineer
% thankyou: Thanks everyone!
% favicon: https://liquidat.files.wordpress.com/2014/02/ansible_logo_round.png

---
title: Do this if you want to play at the end

- `sudo dnf install ansible`
- setup a  passwordless `sshd` server
  - if you want: `docker pull pantinor/centos_sshd` # ~75MB
  - `docker run -it -d --name sshd pantinor/centos_sshd`
- smart config for vi and yaml: `echo "autocmd FileType yaml setlocal ai et ts=2 sw=2" >> ~/.vimrc`

---
title: What's that?

- configuration management tool AND deployment
- alternatives: Chef, Puppet, Salt, **bash** AND Capistrano, Fabric, **bash**
- main differentiator: agentless
- super geeky name (sci-fi)

---
title: The good

- Simple (DSL)
- Tons of libs, just like Camel
- Super popular


---
title: The bad

- YAML ( and I have fat fingers )
- Debugging might be cumbersome
- the DSL has evolved fast. many old scripts look really odd/unreadable
- RH paid ~100M for the acquisition


---
title: The ok

- it's <a href="https://twitter.com/rhatdan/status/898149956657324032">"bash on steroids"</a> Cit. Paolo vs. Dan Walsh
- it's just a script library, with some **smart built-in** and a massive library 
- it doesn't strictly enforce standardization
- requires only SSH (now this is a marketing lie!)
- support for service discovery (inventories, actually)
- good docs
- Ansible Tower/AWX





---

title: Homeworks:

- think what you can use it for
- think what the Fuse team can use it for
- think if we can ship Ansible scripts with our products


---
