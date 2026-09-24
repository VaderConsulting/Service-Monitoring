# Service Monitoring

VB6 Windows service monitor: `Service.dll` (`clsService`) queries, starts, and stops services via SCM APIs; `Service Monitoring.exe` (V1) polls host/service rows and raises Monitoring.dll alerts when a service is down or missing.

**Source last updated:** 2026-08-27 · **Language:** VB6 · **Target:** VB6 Win32 · **Output:** ActiveX DLL, WinForms exe

_Note: original OneDrive LastWriteTime values were wiped to 2026-08-27 by a zip transfer; date above uses best available evidence (headers/copyright where helpful)._

## Solution structure

| Project | Language | Type | Purpose |
|---------|----------|------|---------|
| `Service` (`Dll/Service.vbp`) | VB6 | ActiveX DLL | SCM query/start/stop helpers (`clsService`) |
| `Service Monitoring` (`V1/Service Monitoring.vbp`) | VB6 | WinForms exe | Poll hosts/services and raise Monitoring.dll alerts |

## How to open

Open these `.vbp` files in Visual Basic 6.0 IDE:
- `Dll/Service.vbp`
- `V1/Service Monitoring.vbp`

## Requirements

- Visual Basic 6.0 IDE
- Monitoring.dll (alert helper used by the V1 exe)

## Attribution and provenance

Working copy from my Historical Dev folder `VB/Old/Service Monitoring`.

## License

MIT © 2026 VaderConsulting for Dave Robinson's code. See `LICENSE`.
