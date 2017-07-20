# Running
Make sure you've cleared some space for the flight and any kids/pets are secured !
```
sudo go run drone.go Blaze_XXXXXXX
```

**Note** `sudo` is necessary on Linux, on OSX you should be fine without.

# Pairing with BT (unsure if necessary)

```
pi@raspberrypi:~/workspace/go/src/github.com/johnmccabe/gobot-drone $ sudo bluetoothctl
[NEW] Controller YY:YY:YY:YY:YY:YY raspberrypi [default]

[bluetooth]# agent on
Agent registered

[bluetooth]# default-agent
Default agent request successful

[bluetooth]# scan on
Discovery started
[CHG] Controller YY:YY:YY:YY:YY:YY Discovering: yes
[NEW] Device XX:XX:XX:XX:XX:XX Blaze_XXXXXXX

[bluetooth]# pair XX:XX:XX:XX:XX:XX
Attempting to pair with  XX:XX:XX:XX:XX:XX
[CHG] Device XX:XX:XX:XX:XX:XX Connected: yes
[CHG] Device XX:XX:XX:XX:XX:XX UUIDs:
    xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx
[CHG] Device XX:XX:XX:XX:XX:XX Paired: yes
Pairing successful
[CHG] Device XX:XX:XX:XX:XX:XX Appearance: 0x0080
[CHG] Device XX:XX:XX:XX:XX:XX Icon: computer

[bluetooth]# exit
```