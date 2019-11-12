
##  1. 이해
### 알고 있는 것

- 전체학생수 n, 
- 도난당한 학생들의 번호가 담긴 배열 lost, 
- 여벌의 체육복을 가져온 학생들의 번호가 담긴 배열 reserve
- 학생번호는 체격순-> 내 번호 앞뒤로만 빌려줄 수 있음.

### 모르는 것

- 체육수업을 들을 수 있는 학생의 최댓값.

## 2. 계획

1. 각 학생이 현재 가진 체육복 개수를 표현하는 배열을 만든다. 단, 이 배열의 길이는 전체 학생수와 같다.
2. lost배열에 해당하는 학생의 index - 1 에 해당하는 학생의 개수가 2라면 해당 학생의 체육복 개수를 +1해준다.
3. 빌려준 학생에 해당하면 본인 개수 - 1을 해준다.
3. 만약 index - 1에 해당하는 학생의 체육복 개수가 1이라면 index + 1에 해당하는 학생의 체육복 개수를 확인하고 개수가 2라면 내꺼 + 1, 아니라면 pass
4. 모든 lost 배열에 해당하는 학생에 위의 연산을 반복한다.