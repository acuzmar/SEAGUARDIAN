# SeaGuardian 🛡️

Security Event Analyzer – Matrix‑style Tkinter GUI + FastAPI Dashboard.

## Características principales
* **Análisis de logs CEF/LEEF** con enriquecimiento OSINT (AbuseIPDB, Talos, GreyNoise, OTX).
* **Dashboard en tiempo real** (`/dashboard`) con Chart.js.
* **Integración nativa** con firewalls Palo Alto Networks y Panorama.
* **Exportación** a Excel y PDF.
* **Acciones sugeridas** automáticas según reglas de detección.

## Instalación rápida
```bash
git clone https://github.com/tuUsuario/SeaGuardian.git
cd SeaGuardian
python -m venv venv && source venv/bin/activate   # Windows: .\venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env   # Añade tus API keys
python SeaGuardian.py
```

Abre `http://localhost:8000/dashboard` para el panel.

## Variables de entorno
| Clave | Descripción |
|-------|-------------|
| `ABUSE_TOKEN` | AbuseIPDB API key |
| `GN_TOKEN`    | GreyNoise API key |
| `OTX_TOKEN`   | AlienVault / OTX API key |
| `PAN_TOKEN`   | Palo Alto firewall API key |

## Licencia
MIT © 2025 Alejandro Cuzmar
