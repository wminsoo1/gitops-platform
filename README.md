# gitops-platform

GitOps 실습용 플랫폼 저장소 (#05 역할).

- `bootstrap/root.yaml` : 처음 한 번 `kubectl apply`. 이후 `platform/`을 ArgoCD가 관리
- `platform/projects/`  : 팀원별 배포 허용 범위 (AppProject)
- `platform/apps/`      : 팀원 저장소 목록 (ApplicationSet)
- `.github/workflows/build-push.yml` : 팀원 저장소가 불러 쓰는 공통 CI 템플릿
