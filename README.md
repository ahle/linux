# linux

Sync automatically 
```sh
#!/bin/sh
while inotifywait -r -e modify,create,delete,move sync1; do
    rsync -avz sync1/ sync2/
done
```
