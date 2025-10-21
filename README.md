[README.md](https://github.com/user-attachments/files/23020375/README.md)

# KDP Puzzelboek Webhook

Dit project bevat een eenvoudige Flask-webhook voor het genereren van puzzelboeken.

## Installatie

```bash
pip install -r requirements.txt
```

## Starten

```bash
gunicorn app:app
```

## Webhook endpoint

POST naar `/generate` met JSON-body:
```
{
  "thema": "Kerst",
  "puzzeltype": "woordzoeker",
  "aantal": 20,
  "raster": "15x15",
  "moeilijkheid": "middel"
}
```
