# Hi there, I'm daigato 👋

情報系専攻。クラウド基盤、IaC、自動化まわりの技術を中心に触っています。

---

## Projects

### [kintai](https://github.com/daigato/kintai)
実家の業務向けに作成した、LINE連携の勤怠管理Webアプリ（本番稼働中）。
- **構成**: Cloudflare Workers, Cloudflare D1, Hono, React, LINE LIFF
- **概要**:
  - Workers + D1 のエッジサーバーレス構成により、ほぼゼロコストで運用
  - 外部祝日APIの障害による打刻停止を避けるため、祝日判定ロジックを自作
  - LINE認証と署名検証によるパスワードレス設計

### [weather-bot-infra](https://github.com/daigato/weather-bot)
LINE Botを題材にした、コンテナ化およびAWSインフラのコード化（IaC）検証。
- **構成**: AWS, Terraform, Docker, Python, GitHub Actions
- **概要**:
  - Web API環境をDockerでコンテナ化
  - ネットワークや実行環境をTerraformでコード管理し、構築・破棄の再現性を確保
  - GitHub Actionsによるビルドとデプロイの自動化

---

## Tech Stack
- **Cloud / Edge**: AWS, Cloudflare
- **IaC / Container**: Terraform, Docker
- **Languages**: Python, C
- **CI / CD**: GitHub Actions
