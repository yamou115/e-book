---
description: 這是用於個人學習ELK 架構紀錄 安裝操作步驟
---

# ELK 練習

## 安裝Elasticsearch

Becoming a super hero is a fairly straight forward process:

```
rpm --import https://artifacts.elastic.co/GPG-KEY-elasticsearch
```

添加yum 安裝源

```bash
vi /etc/yum.repos.d/elasticsearch.repo

[elasticsearch]
name=Elasticsearch repository for 7.x packages
baseurl=https://artifacts.elastic.co/packages/7.x/yum
gpgcheck=1
gpgkey=https://artifacts.elastic.co/GPG-KEY-elasticsearch
enabled=0
autorefresh=1
type=rpm-md
```

安裝Elasticsearch 

```text
yum install --enablerepo=elasticsearch elasticsearch
```





