## 1. 이해

- 선행스킬 안에 있는 스킬들은 등장할 땐 반드시 순서대로 배워야 된다.
- 선행스킬 안에 없는 스킬들은 순서에 상관없이 배울 수 있으며
- 선행스킬에 해당하는 스킬들이 반드시 등장해야된다는 제약은 없다.

## 2. 계획

1. skill에 해당하는 문자를 갖고 있는 문자열만 skill_trees에서 찾아낸다.
    1-1. 찾아낸 결과가 아무 것도 없을 시엔 return + 1
2. skill의 조합가능한 스킬트리(부분집합)을 모두 구해서 자료구조에 넣어놓는다.
3. 1에서 추출한 문자열에서 skill(선행스킬)에 해당하는 스킬만 남기고 나머진 지운 문자열을 만든다.
ex) BACDE -> BCD
4. 3에서 나온 결과를 스킬트리 부분집합에 포함되는지 검사한다.
