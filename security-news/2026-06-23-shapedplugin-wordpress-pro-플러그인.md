# Shapedplugin Wordpress Pro 플러그인
- Source: The Hacker News
- Category: security_news
- Original URL: https://thehackernews.com/2026/06/shapedplugin-wordpress-pro-plugins.html
- Published At: unknown
- Collected At: 2026-06-23T11:05:37.577Z
- Notion Page: https://app.notion.com/p/The-Hacker-News-Shapedplugin-Wordpress-Pro-387fc93aec5781029174d33d6e0fc8e0
- Original Title: Shapedplugin Wordpress Pro Plugins
## Summary
공격자들은 ShapedPlugin Pro 업데이트를 백도어하여 자격 증명, 2FA 코드, wp-config.php 데이터 및 WooCommerce 주문 세부 정보를 훔쳤습니다. 알려지지 않은 공격자가 공식 릴리스 채널을 조작하고 백도어 코드를 푸시한 후 ShapedPlugin의 여러 WordPress 플러그인이 공급망 공격으로 인해 손상되었습니다. Wordfence는 지난주 발표된 분석에서 "공격자들은 공식 라이센스 업데이트 채널을 통해 배포되는 Pro 플러그인 릴리스에 백도어 코드를 주입하여 공급업체의 빌드 및 배포 파이프라인을 손상시켰습니다."라고 밝혔습니다. 이 사건은 다음 플러그인에 영향을 미칩니다. - 위에서 언급한 것처럼, 손상은 배포된 Pro 플러그인 빌드에만 영향을 미친다는 점을 강조할 가치가 있습니다…

## Original Description

Attackers backdoored ShapedPlugin Pro updates, stealing credentials, 2FA codes, wp-config.php data, and WooCommerce order details.
## Key Points
- 공격자들은 ShapedPlugin Pro 업데이트를 백도어하여 자격 증명, 2FA 코드, wp-config.php 데이터 및 WooCommerce 주문 세부 정보를 훔쳤습니다.
- 알려지지 않은 공격자가 공식 릴리스 채널을 조작하고 백도어 코드를 푸시한 후 ShapedPlugin의 여러 WordPress 플러그인이 공급망 공격으로 인해 손상되었습니다.
- Wordfence는 지난주 발표된 분석에서 "공격자들은 공식 라이센스 업데이트 채널을 통해 배포되는 Pro 플러그인 릴리스에 백도어 코드를 주입하여 공급업체의 빌드 및 배포 파이프라인을 손상시켰습니다."라고 밝혔습니다.
## Excerpt
알려지지 않은 공격자가 공식 릴리스 채널을 조작하고 백도어 코드를 푸시한 후 ShapedPlugin의 여러 WordPress 플러그인이 공급망 공격으로 인해 손상되었습니다. Wordfence는 지난주 발표된 분석에서 "공격자들은 공식 라이센스 업데이트 채널을 통해 배포되는 Pro 플러그인 릴리스에 백도어 코드를 주입하여 공급업체의 빌드 및 배포 파이프라인을 손상시켰습니다."라고 밝혔습니다. 이 사건은 다음 플러그인에 영향을 미칩니다. - 위에서 언급한 대로 손상은 account.shapeplugin[.]com을 통해 공급업체의 EDD(Easy Digital Downloads) 인프라를 통해 배포된 Pro 플러그인 빌드에만 영향을 미친다는 점을 강조할 가치가 있습니다. WordPress.org의 무료 버전 플러그인은 영향을 받지 않습니다. WooCommerce용 Product Slider Pro와 관련된 공급망 손상에는 CVE 식별자 CVE-2026-49777이 할당되었으며 CVSS 점수는 10.0으로 최대 심각도를 나타냅니다. CVE-2026-10735(CVSS 점수: 9.8)는 전체 사건에 대한 CVE 식별자입니다.