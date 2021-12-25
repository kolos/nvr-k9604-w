## From https://github.com/OpenIPC Wiki:

```bash
# devmem 0x20270110 32 0x60FA0000 ; devmem 0x20270114 8  | awk '{print "CPU temperature: " ((($1)*180)/256)-40}'
CPU temperature: 38.75
```
