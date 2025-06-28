# Quadrant FastAPI Boilerplate

A simple FastAPI boilerplate project that returns "Hello World Quadrant".

## Features

- FastAPI framework with automatic API documentation
- CORS middleware enabled
- Health check endpoint
- Simple and clean project structure

## Setup

1. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

2. **Run the application:**

   ```bash
   python main.py
   ```

   Or using uvicorn directly:

   ```bash
   uvicorn main:app --reload --host 0.0.0.0 --port 8000
   ```

## Usage

Once the server is running, you can access:

- **Main endpoint:** http://localhost:8000/
  - Returns: `{"message": "Hello World Quadrant"}`
- **Health check:** http://localhost:8000/health
  - Returns: `{"status": "healthy", "service": "quadrant-fastapi"}`
- **API Documentation:** http://localhost:8000/docs
  - Interactive API documentation (Swagger UI)
- **Alternative API Documentation:** http://localhost:8000/redoc
  - ReDoc documentation

## Project Structure

```
fastapi-boilerplate/
├── main.py              # Main FastAPI application
├── requirements.txt     # Python dependencies
└── README.md           # This file
```

## Development

The application includes hot reload when using uvicorn with the `--reload` flag, so changes to the code will automatically restart the server.
