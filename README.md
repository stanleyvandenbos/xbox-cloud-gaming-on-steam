# Xbox Cloud Gaming on Steam using Microsoft Edge (flatpak)

-----

## Adding Edge to Steam

Make sure you have Steam (deb) and Microsoft Edge (flatpak) installed.

Open steam and go to Games > Add a Non-Steam Game to My Library...

Select Microsoft Edge and press Add Selected Programs.

Find Microsoft Edge in your Steam Library, right click and change the fields to the settings below.

--

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

--

Launch the 'game', login to your Microsoft (Xbox) account and start playing!

-----

## Extra options

TODO!

[^1]: Optionally you can add `--disable-gpu-vsync --disable-frame-rate-limit` to the launch options to unlock fps.
