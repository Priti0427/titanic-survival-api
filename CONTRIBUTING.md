# Contributing to Titanic Survival Prediction API

Thank you for your interest in contributing!

## Getting Started

1. Fork the repository
2. Clone your fork
3. Create a feature branch: `git checkout -b feature/your-feature`
4. Make your changes
5. Run tests locally
6. Commit your changes: `git commit -m "Add your feature"`
7. Push to your fork: `git push origin feature/your-feature`
8. Open a Pull Request

## Development Setup

### Training Environment
```bash
cd training
docker build -t titanic-training .
docker run -p 8888:8888 -v "$(pwd):/home/jovyan/work" titanic-training
```

### Serving Environment
```bash
cd serving
pip install -r requirements.txt
python app.py
```

## Code Style

- Follow PEP 8 for Python code
- Add docstrings to functions
- Write meaningful commit messages

## Reporting Issues

Please use GitHub Issues to report bugs or request features.
