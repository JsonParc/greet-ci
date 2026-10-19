# greet-ci

명령행 인수로 받은 이름에 인사말을 출력하는 프로그램과 GitHub Actions CI 예제.

## 설치

```bash
uv sync --locked
```

## 실행

```bash
uv run --locked python greet.py Hee   # Hello, Hee!
uv run --locked python greet.py       # Hello, world!
```

## 확인

```bash
uv run --locked pytest -q greet.py
uv run --locked black --check greet.py
uv run --locked flake8 greet.py
uv run --locked mypy greet.py
uv build
```
