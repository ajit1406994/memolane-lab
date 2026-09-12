# memolane-lab

Minimal notes REST API built with Flask

## Usage

```bash
curl -X POST localhost:5000/notes \
  -H 'content-type: application/json' \
  -d '{"title": "first", "body": "hello"}'
```

## Install

```bash
pip install -r requirements.txt
flask --app app run --debug
```

## Features

- Request validation and consistent error shape
- CRUD endpoints for notes
- pytest coverage for the happy paths
- SQLite storage via sqlite3 stdlib

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_api.py
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── app.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
