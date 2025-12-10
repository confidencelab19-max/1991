# 1991

## 배포(Deploy)

이 저장소는 정적 사이트(`index.html`)로 구성되어 있으며, `main` 브랜치에 푸시될 때 자동으로 GitHub Pages로 배포되도록 GitHub Actions 워크플로우를 추가했습니다.

- 워크플로우 파일: `.github/workflows/deploy.yml`
- Jekyll 처리를 방지하기 위해 루트에 `.nojekyll` 파일을 추가했습니다.

배포 확인 방법:

1. `main` 브랜치에 변경사항을 푸시합니다.
2. GitHub 레포지토리의 `Settings > Pages` 또는 `Actions` 탭에서 배포 상태를 확인하세요.

참고: 레포의 Pages 설정은 기본적으로 `gh-pages` 또는 `github-pages` 브랜치 대신 Actions가 업로드한 artifact를 사용해 처리됩니다. 워크플로우가 성공하면 사이트가 자동으로 퍼블리시됩니다.
