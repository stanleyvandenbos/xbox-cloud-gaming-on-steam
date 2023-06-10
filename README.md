# Xbox Cloud Gaming on Steam using Microsoft Edge (Flatpak) 

-----

TARGET
```
"/usr/bin/flatpak"
```

START IN

```
"/usr/bin"
```

LAUNCH OPTIONS[^1]

```
run --branch=stable --arch=x86_64 --command=/app/bin/edge --file-forwarding com.microsoft.Edge @@u @@ --window-size=1024,640 --force-device-scale-factor=1.25 --device-scale-factor=1.25 --kiosk "https://www.xbox.com/play"
```

-----




[^1]: Optionally you can add `--disable-gpu-vsync --disable-frame-rate-limit` to the [launch options](#launch-options) to unlock fps.
