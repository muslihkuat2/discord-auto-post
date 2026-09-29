import os
import requests

WEBHOOK_URL = os.environ["DISCORD_WEBHOOK_1"]

MESSAGE = "Ini adalah pesan auto-post pertama."

response = requests.post(
    WEBHOOK_URL,
    json={"content": MESSAGE}
)

if response.status_code in [200, 204]:
    print("Pesan berhasil dikirim!")
else:
    print("Gagal:", response.status_code, response.text)
