---
title: AWS DEV DAY 2013 
---

## Quick Start

# 10:00  
2019-2023 資訊過於分散 - DX(developer experience)  
reduce cognitive load
1.建立有組織性的架構程式與文件 x
2.易於使用的開發工具
3.自動化

Feedback loops .cognitive load .Flow state
Feedback loops:ai coding companion .devsecops 
cognitive load:docs as code
Flow state:team tools .ai coding companion

aws code catalyst  
建立一個專案並做CICD、開發、測試、正式環境的建立
也許這裡可以學會做開發、測試、上線一條龍含版控

dev & build: 
aws code commit 
aws codebuild
'----------------------------
test:
aws codebuild+third party 
deploy:
aws codedeploy

code & docs
當完成程式 = 完成文件 = docs as code

#####buleprint
#####unifly
#####engagement
#####depth

# 10:50 Generative ai 內容審核.影片搜尋  
內容審核方法(content moderation)
1.explicit nudity 分類
2.suggestion
image > data labeling > train > result  
預訓模型>zero shop capabilities>低再訓(只需要更新問題(question list)與規範(moderation))
whisper>語言轉換(free)

# 11:30
nvida -NeMo 非雲端平台，下載sdk 即可使用


# 13:00
input:all paper 向量體(vector embedding)  

向量資料庫:chroma...(opensource.not incloud search) .postgresql + pgvector(db&search)
尋找最接近的演算法:nearest-neighbors
HNSW(分層往下找).IVF(先預處理分類與類別)
轉向量化模型重點:轉出來的大小.

# 14:33 
「prompt」：原有的模型再訓練，以提示詞(新的題目)再訓
相關技術：Zero-shot.few-shot.chain of thoughts...

fine-tuning
需要更多資料，專注在某個領域，能用prompt方法就不要走到fine-tuning

#　15:15　CDK cloud development kit to definition of infrastrcture
CloudFormation:yaml.json vs cdk 差異：只改配置檔有可能與現行硬體不符以造成死機 cdk提早一點做確認提供適當的配置
cdk = core framework(app.stacks.resources) + cli + construct library

aws vpc = elastic LB + fargate Service (+ ECS task)
傳統作法與cdk差異：
Source Code +　Package = Source Code +　constructs
Artifact = cloud assembly
Process + Resources = stack + Resources
cdk stack(deploy) & cdk construct(build) 運用時機
Synthesis Time 執行的時候才做的事

#####Artifact


### Create a new post
_confix.yml 「default_layout」預設「post」
``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
