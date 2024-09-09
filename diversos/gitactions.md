```yaml
name: CI/CD Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Check out code
        uses: actions/checkout@v2

      - name: Set up Python
        uses: actions/setup-python@v2
        with:
          python-version: '3.x'

      - name: Install dependencies
        run: |
          python -m pip install --upgrade pip
          pip install -r requirements.txt

      - name: Lint code
        run: |
          pip install flake8
          flake8 .

  test:
    runs-on: ubuntu-latest
    needs: build
    steps:
      - name: Check out code
        uses: actions/checkout@v2

      - name: Set up Python
        uses: actions/setup-python@v2
        with:
          python-version: '3.x'

      - name: Run tests
        run: |
          pip install -r requirements.txt
          pytest

  deploy:
    runs-on: ubuntu-latest
    needs: test
    steps:
      - name: Deploy to Heroku
        run: |
          # Comando de deploy para Heroku ou outro serviço de hospedagem
          echo "Deploying application..."
```