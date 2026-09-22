from datetime import datetime, timezone
from pathlib import Path

readme = Path("README.md")

# Heure actuelle en UTC
now = datetime.now(timezone.utc).strftime("%Y-%m-%d %H:%M:%S UTC")

# Lire le README
content = readme.read_text(encoding="utf-8")

# Ajouter une ligne
content += f"\n\n> Dernière mise à jour automatique : {now}\n"

# Écrire le fichier
readme.write_text(content, encoding="utf-8")

print(f"README.md modifié : {now}")
