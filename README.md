# aws-scp-template
下記Zenn記事の個人開発環境向けのSCPテンプレートです。
<ORG_ID>や<SECURITY_TOOLS_ACCOUNT_ID>を誤った値のまま適用すると、組織全体がロックされる可能性があります。
適用前に必ずREADMEの置換ルールを確認してください。

URL：https://zenn.dev/tamago701/articles/69ee7f4d66e089

## 【置換ルール】
| 記号 | SCP名 | 置換対象 | 説明 | 例 |
|-----|--------|----------|------|-----|
| A | scp-deny-org-tamper | `<SECURITY_TOOLS_ACCOUNT_ID>` | myorg-security-toolsのアカウントID | 123456789012 |
| C | scp-deny-data-perimeter | `<ORG_ID>` | Organizations ID | o-xxxxxxxxxx |
| D | scp-deny-org-operation | `<SECURITY_TOOLS_ACCOUNT_ID>` | myorg-security-toolsのアカウントID | 123456789012 |
| E | scp-deny-security-services | `<SECURITY_TOOLS_ACCOUNT_ID>` | myorg-security-toolsのアカウントID | 123456789012 |
| F | scp-deny-s3-protection | `<LOG_BUCKET_NAME>` | CloudTrailログ保存用S3バケット名 | myorg-cloudtrail-logs |
| F | scp-deny-s3-protection | `<SECURITY_TOOLS_ACCOUNT_ID>` | myorg-security-toolsのアカウントID | 123456789012 |
