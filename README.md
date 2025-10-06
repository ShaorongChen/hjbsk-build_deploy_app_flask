# 🧮 Mathematics Problem Solver

A simple Flask web application that performs basic mathematical operations (addition, subtraction, multiplication) via URL parameters.

## 📦 Features

- **Addition**: `/sum?num1=5&num2=3`
- **Subtraction**: `/sub?num1=10&num2=4`
- **Multiplication**: `/mul?num1=6&num2=7`
- **Integer Results**: Automatically converts float results to integers when possible

## 🚀 Getting Started

### Prerequisites
- Python 3.13.x
- Flask

### Installation
```bash
pip install flask
```

### Running the Application
```bash
python server.py
```
The application will be available at `http://localhost:8080`

## 📁 Project Structure
```
.
├── server.py          # Main Flask application
├── Maths/             # Mathematics module
│   └── mathematics.py # Mathematical functions
└── templates/         # HTML templates
    └── index.html     # Main page
```

## 🔧 API Endpoints

### Add Two Numbers
```
GET /sum?num1=<number>&num2=<number>
```

### Subtract Two Numbers
```
GET /sub?num1=<number>&num2=<number>
```

### Multiply Two Numbers
```
GET /mul?num1=<number>&num2=<number>
```

## 📝 Example Usage

- Add: `http://localhost:8080/sum?num1=5&num2=3` → `8`
- Subtract: `http://localhost:8080/sub?num1=10&num2=4` → `6`
- Multiply: `http://localhost:8080/mul?num1=6&num2=7` → `42`