# Quanlinhansu Project

This README provides the necessary steps to get your application up and running.

### What is this repository for? ###

* Human Resource Management System
* Version: 1.0.0

### How do I get set up? ###

#### Configuration

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd quanlinhansu
    ```

2. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install dependencies:
    ```sh
    pip install -r requirements.txt
    ```

#### Database configuration

1. Update the database settings in `quanlinhansu/settings.py`:
    ```py
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.mysql',
            'NAME': 'dbdrf',
            'USER': 'root',
            'PASSWORD': 'bacdz2002',
            'HOST': 'localhost',
            'PORT': '3306',
        }
    }
    ```

2. Apply migrations:
    ```sh
    python manage.py migrate
    ```

#### How to run tests

Run the following command to execute the tests:
```sh
python [manage.py](http://_vscodecontentref_/1) test