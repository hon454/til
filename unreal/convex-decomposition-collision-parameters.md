### Hull Count:
Convex Hull을 여러 조각으로 분리하여 더 복잡한 형태를 근사할 때 사용됩니다. 조각의 개수를 제한함으로써 성능과 메모리 사용량을 조절할 수 있습니다.

### Max Hull Verts:
각 Convex Hull 조각이 가질 수 있는 최대 꼭짓점 개수를 제한합니다. 이것은 각 조각의 복잡도를 제어하며, 너무 큰 값을 설정하면 계산량이 늘어나고 너무 작은 값을 설정하면 정밀도가 떨어질 수 있습니다.

### Hull Precision:
Convex Hull을 생성하기 위해 사용되는 Voxel의 수를 설정합니다. Voxel의 수가 많을수록 더 세밀한 Convex Hull을 생성할 수 있지만, 계산 비용이 증가합니다.
