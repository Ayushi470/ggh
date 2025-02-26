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

## Project Structure

- `/static` - CSS and JavaScript files
- `/templates` - HTML templates
- `/models.py` - Database models
- `/routes.py` - Application routes
- `/ocr_processor.py` - OCR and text processing logic

## Features:

1. **OCR Processing**
   - Upload bill images
   - Extract text using Tesseract
   - Intelligent data extraction for amounts, dates, and items

2. **Bill Management**
   - Store processed bills
   - View bill history
   - Export bills as CSV

3. **Chat Interface**
   - AI-powered responses using Google Gemini
   - Context-aware interactions

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