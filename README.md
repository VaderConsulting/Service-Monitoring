# Service Monitoring

VB6 Windows service monitor: `Service.dll` (`clsService`) queries/starts/stops services via SCM APIs; `Service Monitoring.exe` (V1) polls host/service rows and raises Monitoring.dll alerts when a service is down or missing. Open `Dll/Service.vbp` and `V1/Service Monitoring.vbp` in the VB6 IDE.

**Source last updated:** 2026-08-27 · **Language:** VB6 · **Target:** VB6 Win32 · **Output:** ActiveX DLL, WinForms exe

_Note: original OneDrive LastWriteTime values were wiped to 2026-08-27 by a zip transfer; date above uses best available evidence (headers/copyright where helpful)._

## Solution structure

| Project | Language | Type | Purpose |
|---------|----------|------|---------|
| `Service` (`Dll/Service.vbp`) | VB6 | ActiveX DLL | SCM query/start/stop helpers (`Service.dll`) |
| `Project1` (`V1/Service Monitoring.vbp`) | VB6 | WinForms exe | Poll monitored services and alert on failure |
