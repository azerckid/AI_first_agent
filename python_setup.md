```
uv init your-project
uv venv

copy pyproject.toml
uv sync

uv add firecrawl-py

source .venv/bin/activate
deactivate

uv run main.py


## Jupyter Notebook 사용을 위한 설정

`uv init`은 프로젝트 파일(`pyproject.toml`)만 생성합니다. Jupyter Notebook을 사용하려면 가상환경을 만들고 필요한 패키지를 설치해야 합니다.

1. **가상환경 생성**
   ```
   uv venv
   ```

2. **Jupyter 관련 패키지 설치 (개발용 의존성)**
   ```
   uv add --dev ipykernel jupyter notebook
   ```
   - `ipykernel`: Jupyter가 파이썬 환경을 인식하기 위해 필요
   - `jupyter`, `notebook`: 노트북 실행 및 인터페이스를 위해 필요

3. **VS Code 설정**
   - `Cmd + Shift + P` -> `Developer: Reload Window` (창 새로고침)
   - 노트북 파일(.ipynb) 열기
   - 우측 상단 'Select Kernel' -> 'Python Environments' -> `.venv` 선택
```

## GEMINI
```
uv add google-generativeai python-dotenv
```