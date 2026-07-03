# rag_27

 Version: 0.9.1

 date    : 2026/07/02
 
 update :

***

C++ CLI , RAG Search + Qdrant

* pi-coding-agent
* OpenRouter 
* embedding : Gemini-embedding-001
* gcc version 14.2.0 
* Linux
***
## Image

* RAG APP

![img1](/images/rag_27.png)

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
```

***
* build
```
g++ -std=c++17 -o init init.cpp -lcurl
g++ -std=c++17 -o embed embed.cpp -lcurl -luuid
g++ -std=c++17 -o search search.cpp -lcurl -luuid
```

***
### env value
```
export GEMINI_API_KEY=your-key
```
***
* init-DB
```
./init
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

