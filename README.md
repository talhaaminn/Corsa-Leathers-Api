Corsa leathesr API for company details and integration 

from flask import Flask, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)  # Allow cross-origin requests

corsa_leathers = {
    "name": "Corsa Leathers",
    "location": "Sialkot, Pakistan",
    "address": "Gulshan-e-Tauheed Town Road, Shatabgarh, Sialkot, Pakistan",
    "website": "https://corsaleathers.com",
    "email": "info@corsaleathers.com",
    "phone": "+92-330-2650650",
    "about": "Corsa Leathers, established in 2005, is a Pakistan-Britain-based leading manufacturing company specializing in leather and leather products. We collaborate with global brands, stores, shops, and enterprises to blend business goals and empower brands through custom product development aligned with their unique identity."
}

@app.route("/api/corsa-leathers", methods=["GET"])
def get_corsa_leathers():
    return jsonify(corsa_leathers)

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=5000, debug=True)
    



Corsa Textile API for company details and integration



     from flask import Flask, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)  # Allow cross-origin requests

corsa_textile = {
    "name": "Corsa Textile",
    "location": "Sialkot, Pakistan",
    "address": "Gulshan-e-Tauheed Town Road, Shatabgarh, Sialkot, Pakistan",
    "website": "https://corsatextile.com",
    "email": "info@corsatextile.com",
    "phone": "+92-329-2650650",
    "about": "Corsa Textile is a subsidiary company of Corsa Leathers, Established In 2010. It is a Pakistani-based producer of fabrics, clothing apparel, and accessories. Our mission is to empower brands by collaborating with global brands, stores, and enterprises to deliver custom product development that aligns with their business goals and brand identity."
}

@app.route("/api/corsa-textile", methods=["GET"])
def get_corsa_textile():
    return jsonify(corsa_textile)

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=5000, debug=True)





