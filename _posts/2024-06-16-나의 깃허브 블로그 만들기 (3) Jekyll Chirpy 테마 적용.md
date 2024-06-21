---
title: 나의 깃허브 블로그 만들기 (3) Jekyll Chirpy 테마 적용
date: 2024-06-16 21:30:00 +09:00
categories: [GITHUB]
tags: [GITHUB, BLOG, WINDOWS11, JEKYLL, BUNDLER, CHIRPY, THEME]
---

## 1.Chirpy 테마 다운로드

- [https://github.com/cotes2020/chirpy-starter](https://github.com/cotes2020/chirpy-starter)
- Download ZIP

## 2.chirpy-starter-main.zip

- chirpy-starter-main 파일 압축 풀기
- 파일 탐색기에서 chirpy-starter-main 폴더로 들어가 모두 선택 후 복사, 붙여넣기

## 3.번들 인스톨

```console
bundle install
```

## 4.GitHub Actions를 사용하여 배포하기 위한 처리

```console
bundle lock --add-platform x86_64-linux
```

## 5.Github 빌드와 배포 설정

- Settings -> Pages -> Build and deployment -> source -> GitHub Actions 선택
  ![Chirpy 테마](/assets/posts/2024-06-16/스크린샷 2024-06-16 224139.png)
  _빌드와 배포 설정_

## 6. 배포

```console
git add .
```
```console
git commit -m "Jekyll Chirpy 테마 적용"
```
```console
git push
```