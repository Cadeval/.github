# Contributing to CadEval

Thanks for your interest in contributing to CadEval! We welcome contributions from developers, architects, and engineers of all experience levels.

## Quick Start

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to your branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Development Setup

```bash
# Clone the repository
git clone https://github.com/cadeval/[project-name]
gh repo clone Cadeval/[project-name]

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Unix
.\venv\Scripts\activate   # Windows

# Install dependencies
pip install -r requirements.txt

# Or using uv by [astral](https://docs.astral.sh/uv)
uv venv

# Please note that the venv dir in that case is .venv
# Activation follows the same pattern as above

# A Python version can be requested, e.g., to create a virtual environment with Python 3.11:
# Note this requires the requested Python version to be available on the system. However, if unavailable, uv will download Python for you. See the Python version documentation for more details.
uv venv --python 3.11

# Install a package in the new virtual environment
uv pip install ruff

# Run migrations
python manage.py migrate

# Start development server
python manage.py runserver
```

## Pull Request Guidelines

- Use a clear, descriptive title
- Include relevant issue numbers in the description
- Update documentation as needed
- Add tests for new features
- Follow our coding style (Python: PEP 8)
- Keep changes focused and atomic

## Code Standards

- Use type hints for Python functions
- Document functions and classes using docstrings
- Follow Django best practices
- Maintain test coverage above 80%
- Use meaningful variable and function names

## Working with IFC Files

- Use IFCOpenShell for all IFC operations
- Include sample IFC files for testing
- Document any IFC schema assumptions
- Handle invalid IFC files gracefully

## Testing

```bash
# Run the test suite
make test

# Run formatting
ruff format
```

## Documentation

- Update README.md if adding new features
- Document API changes in the API documentation
- Include docstrings for public methods
- Add comments for complex logic

## Need Help?

- Check our [documentation](https://docs.cadeval.org)
- Tag maintainers in your issue/PR

## Reporting Bugs

- Use the issue tracker
- Include Python/Django/IFCOpenShell versions
- Provide sample IFC files if relevant
- Describe expected vs actual behavior
- Include error messages and stack traces

## Feature Requests

- Check existing issues first
- Explain the use case
- Describe expected behavior
- Be patient and open to feedback

## License

By contributing, you agree that your contributions will be licensed under our project license.

---

Happy coding! 🏗️
