#### character replace
단어 치환(Substitute) - s (substitute)
단어 s는 substitute(치환)의 약자, 그리고 /로 구분하여 old는 단어를 치환할 문자열,  
new는 새롭게 치환한 문자열인데 비어있으면 그 문자열을 삭제한 효과를 가질 수 있습니다. g는 global의 약자로 전체에 적용됨을 의미합니다.  
두번째의 i는 ignore case의 약자로 old의 단어를 검색할때 대소문자 구분하지 않겠다는 것을 의미합니다.  

```
sed 's/://g'
sed 's/://gi'
```
