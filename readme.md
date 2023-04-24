```py
from flask import Flask
app = Flask(__name__)

@app.route('/')
def index():
    return 'hello man'
    
@app.route('/user/<username>')
def username(username):
    return 'i am ' + username

app.run()
```
