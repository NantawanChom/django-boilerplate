# django-boilerplate

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/NantawanChom/django-boilerplate.git
    cd django-boilerplate
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the project dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## Configuration

1. **Create a `.env` file in the project root directory and add the following configuration variables:**

    ```plaintext
    SECRET_KEY=your-secret-key
    DEBUG=True
    ALLOWED_HOSTS=localhost,127.0.0.1
    DATABASE_URL=sqlite:///db.sqlite3  # Use the appropriate database URL
    ```

    You can generate a new secret key using Django's `secrets` module:

    ```python
    from django.core.management.utils import get_random_secret_key
    print(get_random_secret_key())
    ```

2. **Apply the configuration:**

    The project uses `django-environ` to manage environment variables. Ensure you have it installed:

    ```bash
    pip install django-environ
    ```

## Database Setup

1. **Run database migrations to set up the database schema:**

    ```bash
    python manage.py migrate
    ```

2. **Create a superuser (admin) account:**

    ```bash
    python manage.py createsuperuser
    ```

## Running the Server

1. **Start the development server:**

    ```bash
    python manage.py runserver
    ```

2. **Access the project in your web browser:**

    Open [http://localhost:8000](http://localhost:8000) to view the project.

## Running Tests

1. **Run the tests using Django's test framework:**

    ```bash
    python manage.py test
    ```

## Contributing

1. **Fork the repository.**
2. **Create a new branch (`git checkout -b feature-branch`).**
3. **Commit your changes (`git commit -am 'Add new feature'`).**
4. **Push to the branch (`git push origin feature-branch`).**
5. **Create a new Pull Request.**