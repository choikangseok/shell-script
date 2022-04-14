# 유용한 AWK Command
```
# filename을 통한 awk 명령어 활용
$ awk 'pattern' filename
$ awk '{action}' filename
$ awk 'pattern {action}' filename

# 만약 filename을 지정하지 않으면 키보드 입력에 의한 표준입력을 받는다.

# 조건식
$ ls -ltr | awk '$2 < 10'

# 포멧팅 형식 사용 printf
$ ls -ltr | awk '{printf "The filename/dir name is %s\n", $9}'

# awk -f [awk 명령파일] [awk 명령을 적용할 텍스트 파일]

# NR 변수는 1부터 시작해서 하나씩 증가
$ ls -ltr | awk '{printf "%d. The filename/dir name is %s\n", NR, $9}'


# 비교표현식
# 비교표현식 - 어떤 값이 조건에 만족할 경우 수행 
$ ls -ltr | awk ' $9 == "0." {printf "%d. The filename/dir name is %s\n", NR, $9}'

```
