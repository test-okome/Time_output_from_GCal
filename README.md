# Time_output_from_GCal（production_team）
指定した期間のGoogleカレンダーのイベントを取得し、エクセルファイルに出力するPythonスクリプト（今後途中で内容変更あり)

# DEMO

# Features

# Requirement
* google-api-python-client
* google-auth-httplib2
* google-auth-oauthlib
* openpyxl
* configparser


# Installation
```bash
git clone https://github.com/test-okome/Time_output_from_GCal.git
cd Time_output_from_GCal
docker-compose up -d --build
docker-compose exec python3 sh
```
```bash
vi /opt/config.ini
```

```bash
[DEFAULT]
calendar_id = xxxxxxxxxxxxxxxx@group.calendar.google.com
```

GCPの新しいプロジェクトを作成し、OAuth 2.0 クライアント ID作成。認証キー(json)をダウンロード
```bash
/opt/client_secrets.json
```

# Usage
```bash
python get_gcal_info.py --noauth_local_webserver
```

# Note

# Author
* プロジェクト名　production_team
* 作成者 @tomo1833, @test-okome

# License
"production_team" is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).

