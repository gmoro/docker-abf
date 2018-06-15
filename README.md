# docker-abf

How to config user account:
```bash
source envfile
cd rosa-build
rails c
a=User.find_by_email("email")
a.confirmed_at = Time.now
a.save
```
How to add new arch:
```bash
source envfile
cd rosa-build
rails c
Arch.create(name: "arch")
```
