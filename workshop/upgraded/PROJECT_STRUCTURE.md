# upgraded 폴더 프로젝트 파일구조 설명

- **MANIFEST.in**: 패키징에 포함될 파일 목록을 지정하는 설정 파일
- **README.rst**: 프로젝트 설명 파일 (reStructuredText 형식)
- **distribute-0.6.10.tar.gz**: 배포 관련 tarball 파일
- **distribute_setup.py**: 배포/설치 스크립트
- **setup.py**: 패키지 설치 및 배포를 위한 파이썬 스크립트
- **docs/**: 프로젝트 문서 관련 폴더
    - **Makefile**: 문서 빌드용 Makefile
    - **build/**: 빌드된 문서 결과물
        - **doctrees/**: Sphinx 문서 빌드 중간 파일
        - **html/**: HTML 문서 결과물
            - **_sources/**: 각 문서의 원본 텍스트
            - **_static/**: 정적 파일(css, js, 이미지 등)
            - changelog.html, example_usage.html 등: 각 문서별 HTML 파일
    - **source/**: 문서 원본
        - **_static/**: 사용자 정의 CSS 등 정적 파일
        - changelog.rst, example_usage.rst 등: 각 문서별 원본(rst)
        - **conf.py**: Sphinx 문서 설정 파일
- **guachi/**: 주요 파이썬 모듈
    - __init__.py, config.py, database.py: 모듈별 파이썬 코드
    - **tests/**: 테스트 코드
        - test_configmapper.py, test_configurations.py, test_database.py, test_integration.py
- **guachi.egg-info/**: 패키지 메타데이터
    - PKG-INFO, SOURCES.txt, dependency_links.txt, top_level.txt

이 구조는 Python 패키지 및 Sphinx 문서화, 테스트 코드, 배포 관련 파일을 모두 포함합니다.