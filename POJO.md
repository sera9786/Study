# POJO

스프링을 사용하다보면 POJO란 말이 많이 나와서 POJO가 대체 뭐고 왜사용해야하는지에대해 써볼려고한다

POJO(Plain Old Java Object) 오래된 방식의 자바 오브젝트라는 뜻이다

pojo는 특정 규약, 환경에 종속되지않고객체 지향원리에 충실해야한다. 어찌됐든 POJO를 쓰는이유는 

- 코드의 간결함 (비즈니스 로직과 특정환경/low레벨 종속적인 코드를 분리하기때문에 단순하다)
- 자동화 테스트에 유리 (환경에 종속 되지않기때문에 테스트가 자유로움)
- 객체지향 설계에 자유로운 사용 