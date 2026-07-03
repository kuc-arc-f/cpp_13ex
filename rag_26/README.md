# rag_26

 Version: 0.9.1

 date    : 2026/07/02
 
 update :

***

C++ CLI , RAG Search + SQLite DB

* pi-coding-agent
* OpenRouter 
* embedding : Gemini-embedding-001
* gcc version 14.2.0 

***
### Agent Skills

https://github.com/kuc-arc-f/cpp_13ex/tree/main/pi_rag_1

***
## Image

* RAG APP

![img1](/images/rag_26.png)

***
### related

https://pi.dev/

https://pi.dev/docs/latest/quickstart

https://pi.dev/docs/latest/skills

***
* LIB

```
sudo apt install uuid-dev
sudo apt install nlohmann-json3-dev
sudo apt install libcurl4-openssl-dev
sudo apt install libsqlite3-dev
```

***
* build
```
g++ -std=c++17 -I./include -o embed embed.cpp -lcurl -lsqlite3 -luuid
g++ -std=c++17 -I./include -o search search.cpp -lcurl -lsqlite3 -lm
```

***
* table add
```
sqlite3 ./example.db < table.sql
```
***
### env value
```
export GEMINI_API_KEY=your-key
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
### Blog

https://zenn.dev/knaka0209/scraps/c7bc699b98f8a2
