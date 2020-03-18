# Flask-install
We will install and setup flask

Site reference: ```http://mattrichardson.com/Raspberry-Pi-Flask/```

```sudo apt-get install python-pip```

```sudo pip install flask```

```sudo nano flask-hello.py```

```
from flask import Flask
app = Flask(__name__)

@app.route("/")
def hello():
    return "Hello World!"

if __name__ == "__main__":
    app.run(host='0.0.0.0', port=8080, debug=True)
```

I changed the port to 8080. I'm still running Apache that is using the default port 80.

```http://YOUR_RPI_IP_ADDRESS:8080```
