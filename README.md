# --- Go ---
# コンパイルされたバイナリ (cmd直下のファイル名など)
/api
/main
*.exe
*.exe~
*.dll
*.so
*.dylib

# --- SQLC & Tools ---
# sqlcの生成ファイル自体はコミットするのが一般的ですが、
# ツールが一時的に作るキャッシュなどがあれば除外（通常は不要）

# --- Environment ---
# 【最重要】環境変数ファイル
.env
.env.local

# --- Docker ---
# DBのデータがローカルに保存される場合（docker-compose.yamlのvolumes参照）
# もし pgdata/ などのディレクトリを作っているなら除外
/pgdata/

# --- Others ---
.DS_Store


## Credits

This project was built following the tutorial by **Thiago** (Ecom project).  
Special thanks to the original creator for the excellent guidance on Go, SQLC, and clean architecture.

- **Original Video:** [Building a Production API in Golang from Scratch](https://www.youtube.com/watch?v=s3XItrqfccw)
- **Author:** [Thiago's YouTube Channel](https://www.youtube.com/@appliedgo)