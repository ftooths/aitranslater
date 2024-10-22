## AI API 번역기 (v0.1)

### 프로젝트 소개

본 프로젝트는 대용량 텍스트 파일 번역에 어려움을 겪는 사용자들을 위해 개발된 AI 기반 번역기입니다. 기존 AI 번역 서비스들은 텍스트 분량이 많아질수록 프롬프트 용량 제한, 번역 품질 저하 등의 문제를 보였습니다. 이에 본 프로그램은 텍스트 파일을 자동으로 분할하여 번역함으로써 효율성을 높이고, 사용자 편의성을 향상시켰습니다.

### 주요 기능

* 텍스트 파일 드래그 앤 드롭 업로드
* 다양한 AI 번역 모델 지원
* 사용자 지정 가능한 번역 설정 (API 키, 출력 토큰 비율, 배치 토큰 수, 시스템 프롬프트)
* 자동 분할 번역을 통한 대용량 텍스트 처리

### 사용 방법

1. **텍스트 파일 업로드:** 번역할 .txt 파일을 왼쪽 창에 드래그 앤 드롭하여 업로드합니다.
2. **번역 모델 선택:** 오른쪽 상단에서 원하는 AI 번역 모델을 선택합니다.
3. **설정값 지정:** 아래 설정값들을 입력합니다.
    * **api_key:** 발급받은 API 키를 입력합니다.
    * **output_token_magnification:** 출력 토큰 최대 크기를 조절하는 배율입니다. (GPT-4는 1.5~1.6, 그 외 모델은 1.7 권장)
    * **batch_tokens:** 한 번에 번역할 입력 토큰의 근사값입니다. (값이 낮을수록 품질 향상, 비용 증가, GPT-4는 800~1100, 그 외 모델은 700~1000 권장)
    * **system prompt:** 시스템 프롬프트 버튼을 클릭하여 사용자 지정 프롬프트를 설정합니다.
4. **번역 실행:** Start 버튼을 클릭하여 번역을 시작합니다.

### 주의 사항

* **텍스트 형식:** 줄바꿈을 기준으로 문장을 분리하므로, 줄바꿈이 없거나 문단이 너무 긴 경우 번역 오류가 발생할 수 있습니다.
* **테스트 버전:** 현재 테스트 버전으로, 예기치 못한 오류 발생 가능성이 있습니다. 사용에 따른 책임은 사용자에게 있으며, 저용량 파일로 테스트 후 사용하는 것을 권장합니다.
* **중복 실행 방지:** 번역 완료 전 Start 버튼 중복 클릭 시 오류가 발생할 수 있습니다.
* **긴급 정지:** 번역을 멈추는 기능은 아직 구현되지 않았습니다. 번역을 멈추고 싶다면 프로그램을 종료해 주세요
* **같은 파일을 다시 번역:** 같은 파일을 다시 번역하거나, 다른 모델로 번역할 경우, 번역된 파일이 덮어 씌워집니다.

### 향후 업데이트 계획

* 긴급 정지, 중복 실행 방지 추가
* 같은 파일을 다시 번역하면 다른 파일로 저장됨
* 왼쪽 리스트에서 파일 삭제
* 넣은 txt 파일 삭제 기능
* 자동 로어북 생성
* 번역 견본 생성 및 어투 고정 기능
* 병렬 처리를 통한 번역 속도 향상
* 다양한 파일 형식 지원 (.ppt, .xlsx, .docx 등)

**※ 상기 업데이트 계획은 확정된 사항이 아니며, 변경될 수 있습니다.**
