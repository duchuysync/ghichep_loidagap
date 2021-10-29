** xoa log**
 find /proc/*/fd -ls 2> /dev/null | awk '/deleted/ {print $11}' | xargs -p -n 1 truncate -s 0
