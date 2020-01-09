# Flask-Admin for VueJS


Adapted flask-admin for use with VueJS by changing the flask-admin template's delimiters to "[[]]' instead of "{{}}".

Of course, you will need to change the default flask delimiters. One way of doing so is by inheriting the Flask object:

``` python
    class CustomFlask(Flask):
        jinja_options = Flask.jinja_options.copy()
        jinja_options.update(dict(
            variable_start_string='[[', 
            variable_end_string=']]',
        ))
```



## Installation

```
git clone git@github.com:Samy-ib/flask-admin-vueJS.git
cd flask-admin
python setup.py install
```
