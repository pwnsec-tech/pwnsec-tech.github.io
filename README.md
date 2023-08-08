# Overview
PWNSEC Team 기술 블로그입니다. (추가 설명 필요하면 넣을 것)

# Getting Started
로컬 환경에서 블로그 테스트 환경 설정하는 방법을 설명합니다. 
1. install the ruby
    ```
    sudo apt update
    sudo apt install -y make build-essential ruby ruby-dev
    sudo gem install jekyll bundler
    ```
2. update the gem, bundle
    ```
    sudo gem update
    sudo bundle update
    ```

3. execute bundle
    ```
    cd pwnsecy.github.io
    bundle
    ```

4. execute jekyll
    ```
    jekyll serve
    ```
    + localhost:4000 접속

이제 로컬 환경에서 포스팅 글을 수정하고 테스트할 수 있습니다.

# Posting
1. `_posts/` 디렉토리에 `{yy-mm-dd-title}.md` 이름으로 파일을 생성하여 글을 작성합니다.
2. 글 작성 완료 후 commit & push 를 합니다.
3. github 페이지에 접속 후 해당 repository 의 Action 탭을 선택하여 build 까지 완료되었는 지 확인합니다.
4. 확인 후 블로그 주소에서 글이 잘 올라갔는 지 확인합니다.

# 주의 사항
글 작성 시 글 상단에 아래 글을 추가합니다.
```yaml
---
title: TITLE
date: YYYY-MM-DD HH:MM:SS +/-TTTT
categories: [TOP_CATEGORIE, SUB_CATEGORIE]
tags: [TAG]     # TAG names should always be lowercase
---
```