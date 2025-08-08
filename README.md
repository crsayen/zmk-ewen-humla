## ZMK Studio

Enabled via `build.yaml` with:

```yaml
include:
  - board: nice_nano_v2
    shield: humla
    snippet: studio-rpc-usb-uart
    cmake-args: -DCONFIG_ZMK_STUDIO=y
```

Local build example:
```bash
west build -d build/humla_studio -b nice_nano_v2 \
  -S studio-rpc-usb-uart -- -DSHIELD=humla -DCONFIG_ZMK_STUDIO=y
```

In Studio, press your **studio unlock** key to allow editing. If you’re connected over USB, set output to USB (`&out OUT_USB`) before connecting.
