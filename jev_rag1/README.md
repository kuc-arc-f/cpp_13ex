# jev_rag1

 Version: 0.9.1

 date    : 2026/08/10
 
 update :

***

C++ TUI , Jev RAG Search + SQLite DB

* TypeSafe Jev
* embedding : qwen3-embedding-8b
* OpenRouter 
* gcc version 14.2.0 
* LLVM CLang
* make
* Linux
* node 22

***
## Image

* TUI RAG APP

![img1](/images/jev_rag1.png)

***

* .env
```
OPENROUTER_API_KEY=
OPENROUTER_MODEL=deepseek/deepseek-v4-flash-0731
TYPESAFE_API_KEY=
```

***
* LIB

```
sudo apt install uuid-dev
sudo apt install nlohmann-json3-dev
sudo apt install libcurl4-openssl-dev
sudo apt install libsqlite3-dev
```

***
* table add
```
sqlite3 ./example.db < table.sql
```

***
* vector data add
```
./embed ./data
```

***
* build embed
```
g++ -std=c++17 -I./include -o embed embed.cpp -lcurl -lsqlite3 -luuid
```

***
* C++ LIB build
```
make all
```
***
* node-start

```
pnpm i 
npm run start
```
***
### Blog

