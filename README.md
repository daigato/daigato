# Hi there, I'm daigato 👋

クラウドインフラエンジニア / SRE を目指し、IaC（Infrastructure as Code）やコンテナ基盤、エッジコンピューティングの個人検証および本番運用を行っています。

---

## 🛠 Featured Projects（制作実績）

### 1. LINE連携スマート勤怠管理システム（本番運用中）
実家の小規模事業所における労務・勤怠管理課題を解決するためにゼロから設計・実装したエッジ完結型クラウドシステムです。
* **技術スタック**: Cloudflare Workers, Cloudflare D1, Hono, React, Vite, LINE LIFF / Messaging API
* **アーキテクチャ・運用の工夫**:
  * **FinOps（超低コスト運用）**: エッジサーバーレス構成により、実質無料枠（月数十円以下）で本番運用を維持。
  * **SPOF排除**: 外部祝日APIの停止で打刻業務が止まるリスクを排除するため、天文計算を含む祝日判定ロジックを完全内製化。
  * **セキュリティ**: HMAC-SHA256署名検証およびLIFF自動認証によるパスワードレス設計。
* 🔗 [Repository](https://github.com/daigato/kintai) <!-- 公開用クローンリポジトリのURLに合わせて調整してください -->

---

### 2. AWS × Terraform クラウドインフラ自動構築基盤（構築・検証中）
Python製Webアプリケーション（LINE Bot）の実行基盤を、コード（IaC）によって100%再現可能にしたクラウドインフラです。
* **技術スタック**: AWS (App Runner / ECS, VPC, SSM), Terraform, Docker, GitHub Actions, Python
* **アーキテクチャ・運用の工夫**:
  * **環境の完全コード化（IaC）**: ネットワーク構築からコンテナ実行環境、シークレット管理までをTerraformで宣言的に管理。
  * **セキュアなコンテナ設計**: 非rootユーザー実行、マルチステージビルドによるイメージサイズの最小化。
  * **CI/CD自動化**: GitHub Actionsによるコンテナビルド・ECRプッシュ・デプロイパイプラインの統合。
* 🔗 [Repository](https://github.com/daigato/weather-bot) <!-- リポジトリ名に合わせて調整してください -->

---

## 💻 Tech Stack
* **Cloud / Edge**: AWS, Cloudflare
* **IaC / Container**: Terraform, Docker
* **Languages**: Python, C, TypeScript
* **CI / CD**: GitHub Actions
