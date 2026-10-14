# Live Link Face

TouchDesigner sends 61 ARKit curves to Unreal over UDP. MetaHuman drives the face.

## TouchDesigner

- **Live Link** — `Subject`, `Uuid`. The other pages hold the 61 sliders (`Eyeblinkleft` … `Righteyeroll`).
- **UDP Out DAT** `udpout1` — Messaging, the Unreal machine IP, port `11111`.
- **Execute DAT** — `chopexec1.py`, Frame End on. One packet per frame.

## Unreal

- **Plugins** — Live Link and Apple ARKit.
- **Source** — Live Link → Source → Live Link Face.
- **MetaHuman** — Use ARKit Face = On, ARKit Face Subject = `Subject`.
