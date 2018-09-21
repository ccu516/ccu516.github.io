# 如何創建一個Python的虛擬環境

## 為何要創建虛擬環境?
建立一個Python的虛擬環境, 在這裡安裝的所有套件可以被獨立, 不會被互相影響

## Step1. 創建一個虛擬環境
C:\Users\Name\python_practice> python -m venv myvenv
(C:\Users\Name\python_practice = 專案路徑)  (myvenv = 想創建的虛擬環境資料夾名稱)

## Step2. 啟動虛擬環境
C:\Users\Name\python_practice> myvenv\Scripts\activate

## 參考文章:
https://www.openfoundry.org/tw/tech-column/8516-pythons-virtual-environment-and-multi-version-programming-tools-virtualenv-and-pythonbrew

https://tutorial.djangogirls.org/en/django_installation/#virtual-environment

## 如何用BAT來快速啟動虛擬環境?
創建一個BAT檔, 並複製以下程式碼, 並將"專案路徑"與"虛擬環境資料夾名稱"改寫後填入變數, 要使用時啟動BAT檔即可

```
:: Path
set Project_Path=D:\Google Sync\同步用資料夾\程式語言\Python\Crawer_Practice\
set Venv_Folder=myvenv

:: Run Server on Virtual env.
cmd /k "cd /d %Project_Path%%Venv_Folder%\Scripts & activate & cd /d %Project_Path%"
```