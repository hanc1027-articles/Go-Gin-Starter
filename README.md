## Go Gin Starter

### 初始化

- 創建專案
  
```bash
    mkdir {專案名稱}
    cd {專案名稱}
```

- 創建主要檔案

```bash
    touch main.go
```

- main.go必要內容

```go
    package main

    func main() {

    }

```

- 初始化模組

```bash
    go mod init {專案名稱} # 會產生go.mod
```

### 安裝依賴

```bash
    go get github.com/gin-gonic/gin
    # 執行go get時，會自動產生go.sum
```

### 執行

```bash
    go run main.go
    # 或是
    go run .
```

### 參考

- 官方原文：https://go.dev/doc/tutorial/web-service-gin

### 此專案的Endpoints

/albums

- GET – Get a list of all albums, returned as JSON.
- POST – Add a new album from request data sent as JSON.

/albums/:id

- GET – Get an album by its ID, returning the album data as JSON.
