# kat_flaskr

## commands
### build and deploy
```
python3 -m venv venv
pip install -e .

flask init-db

python setup.py bdist_wheel

pip install flaskr-1.0.0-py3-none-any.whl
waitress-serve --call 'flaskr:create_app'
```
### tests
```
pytest
coverage run -m pytest
coverage html
```
### misc
`python -c 'import os; print(os.urandom(16))'`
venv/var/flaskr-instance/config.py
SECRET_KEY = b'_5#y2L"F4Q8z\n\xec]/'