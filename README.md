AWS SAM .Net Hands-on
===================
# 目的 #
AWS サーバーレスアプリケーションモデル (AWS SAM) ハンズオン(.Net) 

# 前提 #
| ソフトウェア   | バージョン   | 備考        |
|:---------------|:-------------|:------------|
| dotnet         |2.1    |             |
| sam            |0.3.0  |             |
| docker         |17.06.2  |             |
| docker-compose |1.21.0  |             |
| vagrant        |2.0.3  |             |

# 構成 #
1. [構築](#構築 )
1. [配置](#配置 )
1. [運用](#運用 )
1. [開発](#開発 )

## 構築
### 開発用仮想マシンの起動・プロビジョニング
+ Dockerのインストール
+ docker-composeのインストール
+ pipのインストール
```bash
vagrant up
vagrant ssh
```

### 開発パッケージのインストール
+ aws-sam-cliのインストール
+ .NET SDKのインストール

```bash
pip install --user aws-sam-cli
sudo rpm -Uvh https://packages.microsoft.com/config/rhel/7/packages-microsoft-prod.rpm
sudo yum update
sudo yum install dotnet-sdk-2.1 -y
```

**[⬆ back to top](#構成)**

## 配置
**[⬆ back to top](#構成)**

## 運用
**[⬆ back to top](#構成)**

## 開発
### アプリケーションの作成
```bash
cd /vagrant
sam init --runtime dotnet
cd sam-app
```

**[⬆ back to top](#構成)**

# 参照 #
+ [.NET Tutorial - Hello World in 10 minute](https://www.microsoft.com/net/learn/get-started-with-dotnet-tutorial#install)