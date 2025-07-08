from flask import Flask, jsonify
from datetime import datetime
import pytz

app = Flask(_name_)

TIMEZONE = 'Asia/Jakarta'  # Ubah di Server 2 jadi Asia/Makassar, Server 3 jadi Asia/Jayapura

@app.route('/time')
def get_time():
    tz = pytz.timezone(TIMEZONE)
    waktu = datetime.now(tz).strftime('%Y-%m-%d %H:%M:%S')
    return jsonify({'time': waktu, 'zone': TIMEZONE})

if _name_ == '_main_':
    app.run(host='0.0.0.0', port=5000)
