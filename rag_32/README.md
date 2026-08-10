# rag_32

 Version: 0.9.1

 date    : 2026/08/10
 
 update :

***

C++ CLI , RAG Search + SQLite DB

* embedding : qwen3-embedding-8b
* OpenRouter 
* gcc version 14.2.0 
* CLang
* make
* Linux

***
## Image

* RAG APP

![img1](/images/rag_32.png)


***
* LIB

```
sudo apt install uuid-dev
sudo apt install nlohmann-json3-dev
sudo apt install libcurl4-openssl-dev
sudo apt install libsqlite3-dev
```
***
### env value

```
export OPENROUTER_MODEL=deepseek/deepseek-v4-flash
export OPENROUTER_API_KEY=
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
* search
```
./search  hello
```

***
* build
```
g++ -std=c++17 -I./include -o embed embed.cpp -lcurl -lsqlite3 -luuid
g++ -std=c++17 -I./include -o search search.cpp -lcurl -lsqlite3 -lm
```

***

* .env
```
OPENROUTER_API_KEY=
OPENROUTER_MODEL=deepseek/deepseek-v4-flash
```

***
* C++ LIB build
```
make all
```
***
* node-start

```
npm i 
npm run start
```

***
### Blog

https://zenn.dev/knaka0209/scraps/f4e50e0fcae420

