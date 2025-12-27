default: pylint pytest

pylint:
<TAB>find . -iname "*.py" \
<TAB>	-not -path "./tests/*" \
<TAB>	-not -path "./.venv/*" \
<TAB>	| xargs -n1 pylint --output-format=colorized || true

pytest:
	@PYTHONDONTWRITEBYTECODE=1 pytest -v --color=yes
