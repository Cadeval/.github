# Welcome to CadEval 🏗️

We're dedicated to developing open-source tools for evaluating and comparing building parameters, leveraging IFCOpenShell for BIM data processing and Django for robust web applications.

## 🎯 Our Mission

To streamline building analysis and comparison through accessible, reliable, and powerful open-source software tools that enhance architectural and engineering decision-making processes. Our tools combine the power of IFC (Industry Foundation Classes) with modern web frameworks to deliver scalable building analysis solutions.

## 🌟 Featured Projects

### BuildingMetrics
Advanced building parameter analysis platform combining IFCOpenShell and Django
- **Tech Stack**: Python, Django, IFCOpenShell, PostgreSQL
- **Features**:
  - IFC model parsing and validation
  - Automated property set extraction
  - Custom parameter calculations
  - RESTful API for building data
  - Real-time 3D visualization

### CompareCAD
Multi-model comparison engine for analyzing building designs
- **Tech Stack**: Django REST framework, IFCOpenShell, Celery
- **Features**:
  - Parallel IFC processing
  - Customizable comparison metrics
  - Automated report generation
  - Version control for building models
  - API-first architecture

### ParametricEval
Real-time parametric modeling evaluation tool
- **Tech Stack**: Django, IFCOpenShell, WebSocket
- **Features**:
  - Live parameter updating
  - IFC export/import
  - Real-time validation
  - Collaborative editing
  - Version history

## 🔧 Technical Framework

### IFCOpenShell Integration
- Native IFC file parsing and creation
- Geometry processing and analysis
- Property set management
- Spatial structure analysis
- Material information extraction
- Building element classification
- Custom property set creation
- Quantity takeoff capabilities

### Django Architecture
- REST API endpoints for building data
- JWT authentication
- Celery task queue for heavy processing
- PostgreSQL for reliable data storage
- Redis for caching and real-time features
- Docker deployment ready
- Comprehensive test coverage
- API documentation with drf-spectacular

## 💪 Contributing

We welcome contributions from architects, engineers, and developers! Here's how you can help:

1. Check out our [contribution guidelines](CONTRIBUTING.md)
2. Browse our [issues](ISSUES.md) for interesting challenges
3. Fork the repository and create a feature branch
4. Submit a pull request with your improvements

### Development Setup
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

## 🤝 Community Standards

* We follow a [Code of Conduct](CODE_OF_CONDUCT.md)
* All interactions should be respectful and professional
* We value diverse perspectives from different disciplines
* We encourage knowledge sharing between architecture, engineering, and development

## 📫 Get in Touch

* [Documentation](https://docs.cadeval.org)

## 📊 Organization Stats

![GitHub Org Stats](https://img.shields.io/github/stars/cadeval?style=flat-square)
![GitHub Org Contributors](https://img.shields.io/github/contributors/cadeval?style=flat-square)
![GitHub Org Repos](https://img.shields.io/github/repos-search/cadeval?style=flat-square)

## 🔌 Supported Integrations

### CAD/BIM Software
* Revit (via IFC export)
* AutoCAD (via IFC export)
* ArchiCAD (native IFC)
* Tekla Structures
* SketchUp (via IFC export)
* Rhino (via IFC export)

### File Formats
* IFC 2x3
* IFC 4
* IFC 4.3
* COBie
* BCF

## 📚 Resources

* [API Documentation](API.md)
* [IFC Integration Guide](IFC-GUIDE.md)
* [Django Setup Guide](DJANGO-SETUP.md)
* [Performance Benchmarks](BENCHMARKS.md)
* [Contributing Guide](CONTRIBUTING.md)

## 🔒 Security

* All projects follow Django security best practices
* Regular dependency updates
* Automated security scanning
* Comprehensive input validation
* Secure IFC file processing

---

© 2024 CadEval. All rights reserved.
