# gcp-py-api-create_vm
Aufgabe zum Erstellen einer VM (Compute Engine) über die Python Client Library `google-cloud-compute`.

## Voraussetzungen
- Zugriff auf ein GCP-Projekt mit aktivierter **Compute Engine API**
- Berechtigung zum Erstellen/Löschen von Compute-Instanzen (z. B. Compute Admin)
- Lokal installiertes `gcloud` (für das Access Token), angemeldet mit dem richtigen Account/Projekt

## Ausführen
1. Öffne das Notebook [create_vm.ipynb](create_vm.ipynb)
2. Führe die Installationszelle aus (installiert `google-cloud-compute`)
3. Erzeuge ein Access Token:
	- `gcloud auth print-access-token`
4. Trage das Token im Notebook in `access_token = '...'` ein
5. Passe `instance_name` an (eindeutig wählen, sonst Namenskollisionen)
6. Führe die Zellen zum Erstellen der VM aus
7. **Cleanup:** Führe am Ende die Delete-Zelle aus, damit keine Ressourcen liegen bleiben
