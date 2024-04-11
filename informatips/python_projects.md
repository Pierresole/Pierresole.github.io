For Python projects, adopting best practices around virtual environments is crucial. 

## 1. Virtual Environments:
Create environment
```bash
python3 -m venv venv
```

Activation: Before working on your project, activate the virtual environment:
```bash
source venv/bin/activate
```

## 2. Dependency Management:

YOU are developper :
```bash
pip freeze > requirements.txt
```

YOU are user
```bash
pip install -r requirements.txt
```

## 3. Project Structure:

```bash
project_name/
├── venv/                    # Virtual environment
├── project_name/            # Source files
│   ├── __init__.py
│   └── main.py
├── tests/                   # Test files
│   ├── __init__.py
│   └── test_main.py
├── README.md
└── requirements.txt         # Dependencies
```



```bash
```
