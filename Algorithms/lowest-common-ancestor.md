# LCA(Lowest Common Ancestor) 최소공통조상

## 알고리즘

- 최상위 조상 정점을 시작으로 DFS(또는 BFS)를 수행하여 각 정점의 깊이와 부모 정점을 저장한다.
  - DFS는 재귀를 사용하여 스택오버플로우가 날 수 있음
- A, B의 공통조상을 구할 경우 더 깊은 노드가 얕은 노드의 깊이에 이를 때까지 부모를 거슬러 올라간다.
- 정점의 부모를 따라 하나씩 올라기 LCA를 찾는다.

## 관련문제

백준 1922 네트워크연결



