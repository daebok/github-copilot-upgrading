# upgraded 폴더 파일 구조 설명

`upgraded` 폴더는 레거시(`legacy`) 폴더의 전체 파일과 디렉터리 구조를 그대로 복사한 디렉터리입니다. 각 파일/폴더의 역할은 다음과 같습니다.

- `MANIFEST.in`: 패키징 시 포함할 파일 목록을 지정하는 설정 파일
- `README.rst`: 프로젝트 설명서 (reStructuredText 형식)
- `distribute-0.6.10.tar.gz`: 예전 Python 패키징 도구인 distribute의 소스 압축 파일
- `distribute_setup.py`: distribute 설치 스크립트 (Python 2.x 레거시 환경에서 사용)
- `setup.py`: 프로젝트 설치 및 배포를 위한 파이썬 스크립트
- `docs/`: 프로젝트 문서 디렉터리 (Sphinx 기반)
- `guachi/`: 주요 소스 코드 디렉터리
    - `__init__.py`: guachi 패키지 초기화 파일
    - `config.py`, `database.py`: 주요 모듈
    - `tests/`: 단위 테스트 코드
- `guachi.egg-info/`: 패키징 메타데이터가 저장되는 디렉터리
- `__pycache__/`: 파이썬 바이트코드 캐시 디렉터리 (Python 3.x에서 자동 생성)

> 이 디렉터리는 레거시 코드를 최신 Python 환경에 맞게 업그레이드하거나, 실험 및 마이그레이션 작업을 안전하게 진행하기 위한 복제본입니다.
