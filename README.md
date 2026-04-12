# 第4回Science of science研究会(2026年) オフィシャルウェブサイト

本リポジトリは、第4回Science of science研究会の公式ウェブサイト用リポジトリです。

- Webpage: https://sciscijp.github.io/scisciconfJP2026

## How to contribute

### 1. Clone

```
git clone git@github.com:ScisciJP/scisciconfJP2026.git
```

### 2. Build with Jekyll

#### Option A: ローカル（bundle）

```
bundle install
```
Note: This step might fail when installing the `nokogiri` gem. If this happens, run `bundle config build.nokogiri --use-system-libraries` and then `run bundle install` again.

Start the jekyll server by running
```
bundle exec jekyll serve
```

-> You can access the test page via http://0.0.0.0:4000/scisciconfJP2026/

#### Option B: Docker

```
docker build -t scisciconfjp2026 .
docker run --rm -p 4000:4000 -p 35729:35729 -v "$PWD:/srv/jekyll" scisciconfjp2026
```

-> You can access the test page via http://0.0.0.0:4000/scisciconfJP2026/

### 3. Edit pages

branchを切ってから、編集してください。
編集する回数の多い箇所は、フォーク元の[こちら](https://github.com/acl-org/acl-2023?tab=readme-ov-file#important-files)に記載があります。以下のファイルが代表的です。

Header: _data/navigation.yml
Body: _pages/*.md

### 4. Push to repository

```
git commit -m "編集内容"
git push origin <branch_name>
```

- push後は、プルリクエストを出してください。
- プログラム委員が確認次第、随時更新します。


# Contact
Contact: [sciscijp@googlegroups.com](mailto:sciscijp@googlegroups.com)<br>
三浦 崇寛(神戸大学): ttmiura225.research@gmail.com<br>
三浦 千哲(東京大学): miura-tchiaki873@g.ecc.u-tokyo.ac.jp