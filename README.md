# 3-tier Architecture 구축 프로젝트

웹의 가장 기본이 되는 3-tier 아키텍처를 Terraform을 이용하여 구축한 뒤, django 애플리케이션을 배포할 예정입니다. 애플리케이션은 대학 수업에서 개발했었던 것을 이용할 것입니다.

**왜 Terraform을 선택했는지에 대하여**

콘솔을 통해 일일히 생성하는 방법도 있지만, 너무 관리하기가 힘들다는 단점이 있습니다. 전에 실수로 만들어둔 NAT 게이트웨이를 삭제하지 않았더니 사용하지않았음에도 5만원이 청구되었던 경험이 있습니다. 그래서 코드로 인프라를 관리하면 만들었다가 한 번에 삭제하기도 유용하다는 생각이 들어서 IaC를 사용해보고자 생각했습니다.

그 중에서도 Terraform을 선택한 이유는 오픈소스이기 때문에 커뮤니티가 활발해서 정보를 얻기 쉽다는 점과, 코드가 간단하고 직관적이어서 빠르게 학습할 수 있을 것 같았기 때문입니다.
