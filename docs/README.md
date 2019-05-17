# 说明

> [本文档使用docsify编写](https://docsify.js.org/#/)

# 安装nodejs、docsify
安利一个Windows package manager [Chocolatey](https://chocolatey.org/)  
在cmd运行（管理员权限）
```
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

或者在PowerShell运行（管理员权限）
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

安装完成之后开始安装nodejs  
```
choco install nodejs
```

安装docsify
```
npm i docsify-cli -g
```
# 创建文档模板
创建一个目录，进入目录，执行如下命令生成文档模板  
```
docsify init ./docs
docsify serve docs
```

浏览器访问 http://127.0.0.1:3000 就可以看到文档了

# 托管到github
github创建仓库