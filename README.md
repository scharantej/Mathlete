 ## Design

The Flask application will consist of the following HTML files:

* `index.html`: The home page of the application. This page will contain links to the different math lessons.
* `lesson1.html`: The first math lesson. This page will contain a video explaining the lesson, as well as some practice problems.
* `lesson2.html`: The second math lesson. This page will contain a video explaining the lesson, as well as some practice problems.
* `lesson3.html`: The third math lesson. This page will contain a video explaining the lesson, as well as some practice problems.

The Flask application will also have the following routes:

* `/`: The home page of the application.
* `/lesson1`: The first math lesson.
* `/lesson2`: The second math lesson.
* `/lesson3`: The third math lesson.

## Implementation

The following code is the implementation of the Flask application:

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def index():
  return render_template('index.html')

@app.route('/lesson1')
def lesson1():
  return render_template('lesson1.html')

@app.route('/lesson2')
def lesson2():
  return render_template('lesson2.html')

@app.route('/lesson3')
def lesson3():
  return render_template('lesson3.html')

if __name__ == '__main__':
  app.run(debug=True)
```

## Testing

To test the Flask application, you can run the following command:

```
python app.py
```

This will start the Flask application on port 5000. You can then access the application by visiting http://localhost:5000 in your web browser.