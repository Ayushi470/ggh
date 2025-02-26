# Document Processing System with OCR

A web application designed to streamline document processing for employees, featuring advanced Python-based OCR capabilities and intelligent data extraction.

## Features

- OCR-powered bill processing using Tesseract
- Natural Language Processing for data extraction
- Interactive chat interface with AI responses
- Bill management and reporting
- Data visualization and export capabilities

## Tech Stack

- **Backend**: Flask (Python)
- **Database**: PostgreSQL with SQLAlchemy
- **OCR Engine**: Tesseract with Python bindings
- **NLP**: spaCy for text processing
- **Frontend**: Bootstrap with dark theme
- **AI Integration**: Google Gemini API for chat

## Environment Variables Required

Make sure to set up the following environment variables:
- `DATABASE_URL`: PostgreSQL database connection URL
- `GEMINI_API_KEY`: Google Gemini API key for chat functionality
- `SESSION_SECRET`: Secret key for Flask sessions

## Required Dependencies

```bash
# Core Web Framework
flask>=3.1.0
flask-sqlalchemy>=3.1.1
flask-login>=0.6.3
flask-wtf>=1.2.2
gunicorn>=23.0.0

# Database
psycopg2-binary>=2.9.10
sqlalchemy>=2.0.38

# OCR and Image Processing
pytesseract>=0.3.13
pillow>=11.1.0

# NLP and Text Processing
spacy>=3.8.4
numpy>=2.2.3

# Additional Utilities
email-validator>=2.2.0
flask-pymongo>=3.0.1
google-generativeai>=0.8.4
werkzeug>=3.1.3
trafilatura>=2.0.0
```

## Setup Instructions

1. Install required system dependencies:
   - Python 3.11
   - PostgreSQL
   - Tesseract OCR

2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up environment variables (mentioned above)

4. Initialize the database:
   ```bash
   flask db upgrade
   ```

5. Run the application:
   ```bash
   python main.py
   ```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the MIT License.