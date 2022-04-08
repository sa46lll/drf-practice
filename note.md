### Django Rest Framework

>  DRF Router
- SimpleRouter
  - 표준 셋으로 list, create, retrieve, update, partial_update 그리고 destroy 작업에 대한 경로가 포함함
  - viewset은 @action 데코레이터를 사용하여 라우팅할 추가 메서드를 표시
- DefaultRouter
  - SimpleRouter과 유사하지만 모든 list views에 하이퍼링크를 포함하는 응답을 반환하는 기본 API Root view를 포함함
  - 포맷 스타일 형식을 접미사나 query_string에 대한 경로 생성
    - ex) localhost:8000/api2/users/ **?format=json**
    - localhost:8000/api2/users **.json**

> ViewSet
- 상속 관계
  - View > APIView > GenericAPIView
- ReadOnlyModelViewSet
  - 목록 조회 & 특정 레코드 조회 (get만 가능)
- ModelViewSet
  - 목록 조회 & 특정 레코드 생성/조회/수정/삭제 전부 자동으로 만들어 줌.
    - CreateAPIView
    - ListAPIView
    - RetrieveAPIView
    - UpdateAPIView
    - DestroyAPIView
  - ViewSet
    - 자동으로 만들지마! 내가 다 만들께

> 참고문서
- [DRF 참고문서](https://www.cdrf.co/)
- [CBV 참고문서](https://ccbv.co.uk/)