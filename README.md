# langchain_practice
랭체인을 연습하기 위한 예제들 입니다. 많이 사용하세요.

# 랭체인 (LangChain)

랭체인이 가지는 모듈에 대해 설명하고, 체인을 어떻게 실현하나 보면서 기본적인 것만 **빠르게** 훑어볼려고 합니다.

랭체인(LangChain)은 대규모 언어 모델(LLM)을 기반으로 한 어플리케이션 개발을 위한 프레임워크로, 언어 모델을 사용한 다양한 작업을 효과적으로 수행할 수 있게 해주는 도구입니다. 

랭체인은 여러 모듈로 구성되어 있으며, 이 모듈들이 함께 작동하여 언어 모델과 데이터 소스를 효과적으로 연결하고, 애플리케이션의 작업 흐름을 체계적으로 관리합니다. 

랭체인은 모듈들 간의 조합을 통해 언어 모델과 데이터 소스를 효과적으로 연결하고, 이를 통해 다양한 작업을 수행합니다. 각 모듈은 모듈화된 추상화 및 구현을 통해 유연성을 제공하며, 사용자는 구성 요소를 조합하여 기존 체인을 맞춤설정하거나 새로운 체인을 생성할 수 있습니다.

에이전트 모듈을 통해 사용자의 입력으로 부터 답변으로 요구되는 것을 추론하고 필요한 도구를 선택해 실행하므로서 최적의 답변을 도출합니다.

에이전트 내부적으로 답변이 불충분 하다 판단되면 다시 추론과 행동을 반복함으로서 복잡한 작업을 높은 정확도로 구현 할 수 있습니다. 

### 주요 모듈

**모델 I/O (입출력):** 언어 모델과의 상호작용을 관리하며, 프롬프트를 조작하고 언어 모델의 출력에서 정보를 추출합니다.

**데이터 연결:** 애플리케이션별 데이터를 로드, 변형, 저장 및 쿼리하기 위한 필수 빌딩 블록을 제공합니다.

**체인:** 작업의 호출 순서를 구축하고 체인으로 연결된 다양한 구성 요소를 효율적으로 관리합니다.

**에이전트:** 상위 지시문을 받으면 어떤 툴을 사용할지 결정하여 체인을 유연하게 조작합니다.

**메모리:** 대화형 시스템이 과거 메시지에 직접 액세스할 수 있도록 해주는 기능을 제공합니다.

**콜백:** 체인의 중간 단계를 기록하고 스트리밍하여 로깅, 모니터링 및 기타 작업에 활용됩니다.  **(다음기회에)**

### 랭체인 사용 사례

랭체인은 다양한 사용 사례에 적용될 수 있습니다. 이에는 문서에 대한 Q&A, 구조화된 데이터 분석, API 통합, 코드 이해, 에이전트 시뮬레이션, 챗봇 개발, 코드 작성, 데이터 추출,그래프 데이터 분석, 멀티 모달 출력, 자가 검사, 요약, 태깅 등이 포함됩니다.

또한 랭체인은 다양한 통합을 지원하여 콜백, 챗 모델, 문서 로더, 데이터베이스, 검색 방법, 텍스트 임베딩 모델, 에이전트 툴킷, 툴, 벡터 저장소 등을 활용할 수 있도록 제공됩니다.



## 라마인덱스 vs 랭체인

![](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FrdIRx%2Fbtszy3Jaw8y%2FjdbbN6j4jjRqZqK4C9EnJK%2Fimg.png)

이와 비슷한 라이브러리가 라마 인덱스(구, GPT 인덱스)가 존재하지만, 라마 인덱스가 랭체인 라이브러리를 기반으로 구축된 애플리케이션입니다.

라마 인덱스를 잘 다루기 위해서는 랭체인을 익힐 필요가 있습니다.

- Langchain은 초기 프로젝트 시작 및 최신 기술의 구현에 적합하며 빠르게 적용할 수 있음.
- llama index는 데이터 쿼리와 정보 합성에 중점을 두며, 복잡한 메모리 관리가 필요한 경우 적합.


- Langchain의 사용자 인터페이스는 더 간편하고 개발자 커뮤니티가 큼. 
- llama index는 메모리 구조에 중점을 두며, 쿼리 능력이 강화됨.


- Langchain는 간단하게 시작하기 쉬우며 예제와 자료가 풍부함.
- llama index는 복합 에이전트 구성과 유연한 메모리 구조에 더 적합.


- 프로젝트 방향을 설정하는 단계일 때, Langchain을 시작하는 것이 권장됨. 
- llama index는 고급 사용자나 명확한 프로젝트 요구사항이 있는 경우에 적합.

## 진행순서
어디까지 할지는 모르겠지만, 되는 대로 진행 예정

1. OpenAI 라이브러리를 통한 랭체인 기본 펑션들의 사용 법을 설명
   1. 챗메세지
   2. 프롬프트 탬플릿
   3. 아웃풋 파서
   4. 체인 연결
   5. 텍스트 분할
   6. 문서 다루기
   7. 벡터인덱스
   8. 예제 선택
   9. 메모리 사용
   

2. 커스텀 사용법
   1. 허깅페이스 파이프라인 LLM
   2. 커스텀으로 LLM 구동
   3. 커스텀 아웃풋 파서
   4. QA 리트리버
   5. 요약기

3. 질문 없음
