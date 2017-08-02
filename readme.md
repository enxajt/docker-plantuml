# how to use
```
docker run -p 8000:8000 -p 35729:35729 -v $(pwd):/plantuml/src -v $(pwd):/plantuml/dst --rm -it plantuml
gulp
http://localhost:8000/dst/dev-cycle-member.html
```
LiveReload uses port 35729
gulp task, .src~ in task は非同期、並列実行。
it's impossible to run gulp on docker on VM with gulpfile on XPS

# virtual box setting
TCP
HostIP:empty
HostPort:35729
GuestIP: empty
GuestPort: 35729

TCP
HostIP:empty
HostPort:8000
GuestIP: empty
GuestPort: 8000
