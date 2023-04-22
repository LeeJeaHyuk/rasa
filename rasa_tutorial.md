참고한 유튜브 https://www.youtube.com/watch?v=06CCCvyugwg

중요 파일
1. rasa/data/nlu.yml
    - nlu.yml 파일은 Rasa 프로젝트에서 자연어 이해(NLU) 모델을 학습시키기 위한 훈련 데이터를 정의하는 파일입니다. NLU 모델은 사용자의 메시지를 이해하고 의도(intent)와 엔티티(entity)를 추출하는 데 사용됩니다.

    - nlu.yml 파일은 YAML 형식으로 작성되며, 각 문장은 샘플이라고 불리는 사용자 메시지와 해당 메시지가 나타내는 의도 및 관련 엔티티의 예제로 구성됩니다

    - 구성 요소
        - intent는 사용자가 전달하는 문장에 담긴 의도를 나타내며, 
            - 오늘 서울 날씨 어때? -> intent : wheather_require
        - entities는 문장에 포함된 개체(entity) 정보를 나타냅니다.
            - 오늘 서울 날씨 어때? -> entities : location(서울)
        - example란 사용자 발화의 실제 예시를 말합니다.    
        - slot
            - 사용자와 대화 할 때 사용자와의 문맥을 이해하기 위해 저장되는 정보
            - entity를 slot으로 지정할 수도 있다
2. rasa/data/stories.yml
3. rasa/domain.yml

- 어떤 것을 만드는지
    - 챗봇이 개인의 일상 정보와 연동되면 훨씬 삶의 안락함이 나올 수 있을 것
    - 캘린더(일정), 가계부 등과 연동해서 해당 정보를 쉽게 불러올 수 있도록 하는 것