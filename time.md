# Time

Make the containers use the same timezone as the underlaying host.

```
  volumeMounts:
  - name: tz-config
    mountPath: /etc/localtime
volumes:
  - name: tz-config
    hostPath:
      path: /usr/share/zoneinfo/Europe/Stockholm
```
