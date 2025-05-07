# StudyBuddy

StudyBuddy is a Django-based web application designed to help students organize their study sessions, track progress, and collaborate with peers. This platform integrates productivity tools with community features to foster effective learning environments.

![StudyBuddy Banner](https://github.com/kartikeya-datta/StudyBuddy/raw/main/static/images/studybuddy-banner.png)

## 🚀 Features

* **User Authentication**: Secure registration and login system using Django's authentication framework
* **Custom User Profiles**: Personalized dashboards displaying study goals, progress, and achievements
* **Study Session Management**: Create, edit, and delete study sessions with customizable timers
* **Progress Tracking**: Visual representations of study habits and accomplishments
* **Community Interaction**: Connect with fellow learners, join study groups, and share resources
* **Responsive Design**: Mobile-friendly interface ensuring accessibility across devices

## 🛠️ Tech Stack

* **Backend**: Django (Python)
* **Frontend**: HTML, CSS, JavaScript
* **Database**: SQLite (default), with the option to switch to PostgreSQL or MySQL
* **Version Control**: Git

## 📂 Project Structure

```
StudyBuddy/
├── base/                   # Core application logic
│   ├── admin.py           # Admin configuration
│   ├── apps.py            # App configuration
│   ├── forms.py           # Form definitions
│   ├── models.py          # Database models
│   ├── tests.py           # Test cases
│   ├── urls.py            # URL routing
│   └── views.py           # View functions
├── customusermodel/        # Custom user model implementation
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── static/                 # Static files (CSS, JS, images)
│   ├── css/
│   ├── js/
│   └── images/
├── templates/              # HTML templates
│   ├── base.html
│   ├── main.html
│   └── components/
├── studybud/               # Main project configuration
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── manage.py               # Django's command-line utility
├── requirements.txt        # Project dependencies
├── .gitignore              # Git ignore file
├── LICENSE                 # MIT License
└── db.sqlite3              # Default SQLite database
```

## ⚙️ Installation

1. **Clone the repository**:

```bash
git clone https://github.com/kartikeya-datta/StudyBuddy.git
cd StudyBuddy
```

2. **Create and activate a virtual environment**:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**:

```bash
pip install -r requirements.txt
```

4. **Apply migrations**:

```bash
python manage.py migrate
```

5. **Create a superuser** (optional):

```bash
python manage.py createsuperuser
```

6. **Run the development server**:

```bash
python manage.py runserver
```

7. **Access the application**:
   - Navigate to `http://127.0.0.1:8000/` in your web browser
   - Admin interface: `http://127.0.0.1:8000/admin/`

## 🧪 Testing

To run tests, use Django's testing framework:

```bash
python manage.py test
```

## 🔄 Database Configuration

By default, StudyBuddy uses SQLite. To use PostgreSQL or MySQL:

1. Install the appropriate database adapter:
   - PostgreSQL: `pip install psycopg2-binary`
   - MySQL: `pip install mysqlclient`

2. Modify the `DATABASES` setting in `studybud/settings.py`.

## 📊 Demo

![Dashboard Demo](https://github.com/kartikeya-datta/StudyBuddy/raw/main/static/images/dashboard-demo.png)

## 🔧 Environment Variables

Create a `.env` file in the root directory with the following variables:

```
DEBUG=True
SECRET_KEY=your_secret_key
DATABASE_URL=sqlite:///db.sqlite3
```

For production, set `DEBUG=False` and use a proper database URL.

## 📱 API Documentation

API endpoints are available at `/api/v1/`. Documentation can be accessed at `/api/docs/`.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

Please ensure your code adheres to the project's coding standards and includes appropriate tests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [Django](https://www.djangoproject.com/)
- [Bootstrap](https://getbootstrap.com/)
- [Chart.js](https://www.chartjs.org/)
- [Font Awesome](https://fontawesome.com/)

## 📬 Contact

For questions or feedback, please reach out via:

- GitHub Issues: [https://github.com/kartikeya-datta/StudyBuddy/issues](https://github.com/kartikeya-datta/StudyBuddy/issues)
- Email: [example@example.com](mailto:example@example.com)

## 📊 Project Status

StudyBuddy is currently in active development. New features and improvements are being added regularly.
