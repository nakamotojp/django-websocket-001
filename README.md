# django-websocket-001
django-websocket-001 sample

## cloud9 

### python3.9.18

https://qiita.com/hir1524/items/41676432a9b353ba1766

```
sudo rm /etc/alternatives/python
sudo ln -s /usr/bin/python3.9 /etc/alternatives/python
vi ~/.bashrc
```

#### vimモード

```
# User specific aliases and functions
alias python=python39
```

### python --version

```
python --version
```

### 基本ライブラリ

```
sudo apt update
udo apt -y install libbz2-dev liblzma-dev

```

### 仮想環境

```
python -m venv venv
source venv/bin/activate
```

### Djangoインストール

```
pip install Django
```

### startproject

考え方：https://docs.djangoproject.com/ja/5.0/intro/tutorial01/

`.` だとカレントディレクトリに `manage.py` が生成される

```
django-admin startproject config .
```

#### プロジェクトフォルダを作成する場合


```
django-admin startproject プロジェクトフォルダ名
```

### アカウント管理用アプリを生成

Djangoでは、 `manage.py` があるディレクトリで、 `startapp` することで機能別のディレクトリを生成する設計

```
django-admin startapp accounts
```

#### error

```
django.core.exceptions.ImproperlyConfigured: AUTH_USER_MODEL refers to model 'accounts.User' that has not been installed
```
