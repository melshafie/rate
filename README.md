
# Rate 
rate is API that tracks exchange rates.


1. Clone or download this repo.

2. Create a virtual environment on Linux or Mac:  
`python3 -m venv  ~/.virtualenvs/flextock`
3. Activate the virtual environment on Linux or Mac:  
`source ~/.virtualenvs/flextock/bin/activate`

4. Install requirements in the virtualenv:  
`pip3 install -r requirements.txt`
5. Make Django database migrations:
`python manage.py makemigrations`
then: `python manage.py migrate`


Create Superuser for Admin:
1. `python manage.py createsuperuser`
2. ADMIN USER
```
username: admin
password: 123
```

Go  to: `http://localhost:8000/admin/`

API Endpoints:

1. Endpoint: `/rate`
2. Method: `GET`
3. Parameters: `?date=2020-10-07&from_currency=usd&to_currency=eur`
- Full Endpoint: `http://localhost:8000/rate/?date=2020-10-05&from_currency=usd&to_currency=eur`

