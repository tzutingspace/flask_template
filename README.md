# Templates

### Setup
- Modify `template.py`
- Run `sh init_setup.sh` or  `source init_setup.sh`  

### Notes
來源文章是用 venv 當作 virtual environment 管理, 我改為用 conda 來管理
- 每次 activate 要用 `source venv/bin/activate`
- 而且他的方式將 modules 放在當下資料夾下

### 資料夾結構說明

#### Root 下有以下 file
1. .env (for project secrets)
2. DockerFile
3. .gitignore
4. app.py (Application starting point)
5. README.md
6. init_setup.sh (Automation script for setting up environment)
7. template.py (Automation script to create folders and files in it) -> 啟動專案後 就不需要了

#### 主要 app 放在 src (或是你可以取你想要的名字, 常見的有 app, api, ...)
#### 通常裡面會有 以下 folder
1. config
2. controllers
3. middlewares
4. models
5. services
6. utils (個人會放一個 folder)

#### 通常裡面會有 以下 file
6. src/routes.py 
7. src/utils.py (小型專案, 原文作者用一個 file)










#### Reference:
- [Flask API Folder Guide 2023](https://ashleyalexjacob.medium.com/flask-api-folder-guide-2023-6fd56fe38c00)