FFMPEG
=========

Install latest version of FFMPEG.

Requirements
------------

Refer to the official FFMPEG documentation.

Role Variables
--------------

Required variable: `ffmpeg_repo`<br>
Example: `ffmpeg_repo: ppa:jonathonf/ffmpeg-3`

Dependencies
------------

N/A

Example Playbook
----------------
```
$ ansible-galaxy install stockhausenj.ffmpeg
$ ansible-playbook -i inventory.yaml install-ffmpeg.yaml -u <ssh-user> -K
```
```
- hosts: all
  become: true
  roles:
    - include_role:
        name: stockhausenj.ffmpeg
      vars:
        ffmpeg_repo: 'ppa:jonathonf/ffmpeg-3'
```

License
-------

MIT
