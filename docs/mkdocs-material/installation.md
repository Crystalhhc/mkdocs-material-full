# Installation


## Set up repository in github
- Create a new Repo in github

## Clone repo to your local
```sh
gh repo clone Crystalhhc/notebook
cd notebook

```
## 在root建立`requirements.txt`
```sh
├─ notebook
│  └─ requirements.txt
└─ 

```
## Python Env Setting
```sh
├─ notebook
│  └─ init_setup.sh
│  └─ requirements.txt
└─ 
```

```sh title="init_setup.sh"
notebook%conda create --prefix ./env python=3.8 -y
notebook%source activate ./env
notebook%pip install -r requirements.txt
```
then execute init_setup.sh in terminal:

```
notebook%bash init_setup.sh
```
- 與Github 同步
- 啟動環境

```bash
notebook%conda activate ./env

```
- 建立mkdocs instance
```sh
mkdocs new .
```
執行完會新增一個檔案`mkdocs.yml`檔案, 及 `doc\`目錄

```sh
├─ notebook
│  └─ init_setup.sh
│  └─ docs
│  └─ mkdocs.yml
│  └─ requirements.txt
└─ 
```
