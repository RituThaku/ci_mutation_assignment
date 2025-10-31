# CI + Mutation Testing Assignment

## Part 1: Continuous Integration (CI)
- Implemented with **GitHub Actions**
- Runs **PyTest** automatically for every push or pull request
- Generates **test coverage** report

## Part 2: Mutation Testing
- Done using **MutPy**
- Measures test suite strength using mutation score

### How to Run Locally
```bash
pip install -r requirements.txt
pytest --cov=app --cov-report=term-missing
mut.py --target app/calculator.py --unit-test tests/test_calculator.py --runner pytest --report-html report.html
```
