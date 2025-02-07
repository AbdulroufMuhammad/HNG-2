# FastAPI Application

This is a simple FastAPI application that includes CORS middleware and a single endpoint.

## Features

- **CORS Middleware**: Allows all origins, methods, and headers.
- **Root Endpoint**: Returns email, current datetime in ISO 8601 format (UTC), and a GitHub URL.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/AbdulroufMuhammad/HNG-2.git
    cd HNG-2
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install fastapi uvicorn
    ```

## Usage

1. Run the application:
    ```bash
    uvicorn main:app --reload
    ```

2. Open your browser and navigate to `http://127.0.0.1:8000` to see the root endpoint response.

## Endpoints

- `GET /`: Returns a JSON response with the following fields:
  - `email`: Contact email.
  - `current_datetime`: Current datetime in ISO 8601 format (UTC).
  - `github_url`: URL to the GitHub repository.

## Example Response

```json
{
    "email": "abdulraufmuhammad28@gmail.com",
    "current_datetime": "2023-10-05T12:34:56Z",
    "github_url": "https://github.com/AbdulroufMuhammad/HNG-2"
}
```

## License

This project is licensed under the MIT License.