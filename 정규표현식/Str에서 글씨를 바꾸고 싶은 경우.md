정규 표현식 진행 중 해당 문자에 포함되는 글자를 바꾸고 싶을 경우가 많다.
그때는 해당 코드를 사용해주면 된다.
```python
import re
text = 010-0304-2020
change_text = re.sub("[^0-9a-zA-Z]","*",text)
```
여기서 [^0-9a-zA-Z]의 뜻은 "숫자, 영어 소문자 대문자를 제외한" 것은 \*로 바꾸어 준다 라는 뜻이다.
