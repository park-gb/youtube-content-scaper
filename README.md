# Python 기반 유튜브 콘텐츠 Scraper V.1.0.1
[Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Google Chrome](https://img.shields.io/badge/Google%20Chrome-4285F4?style=for-the-badge&logo=GoogleChrome&logoColor=white)

## Update Log
### (1) 2022-10-11
- 콘텐츠 조회수 및 업로드일 추출 추가

## 1. 주요 기능
- 유튜브 내 검색 결과의 콘텐츠 정보 Scrap
- 수집 데이터 종류
  - 콘텐츠 제목
  - 콘텐츠 하이퍼링크
  - 조회수
  - 업로드일(i.e., 현재 기준 경과일)
- 수집한 데이터는 데이터프레임 형태로 포맷팅(`data/content_total.csv`)

<img width="844" alt="src" src="https://user-images.githubusercontent.com/80144296/195092049-c7f68210-236b-4a69-9073-ea8860b392f2.png">

## 2. 실행방법 
### (1) 패키지 설치
#### 방법 1. pipenv 활용(권장)
- Pipfile 내 모든 패키지 자동 설치
```python
$ pipenv install
```
- pipenv 사용법 관련 [문서](https://heytech.tistory.com/320)

#### 방법 2. pip 활용
```
$ pip install bs4==0.0.1
$ pip install selenium==4.1.2
$ pip install webdriver-manager==3.5.3
$ pip install pandas==1.4.1
$ pip install numpy==1.22.2
```

### (2) 검색 키워드 설정
- 유튜브에서 검색할 키워드를 ```SEARCH_KEYWORD``` 변수 내 문자열로 입력

## 3. 전체 파일구조
``` bash
├─youtube-content-scraper
│ README.md
│ Pipfile
│ Pipfile.lock
│ requirement.txt
│  ├─src
│  │      scraper.ipynb
│  └─data
│         content_total.csv
```

## 4. 실행 결과
![ezgif com-gif-maker](https://user-images.githubusercontent.com/80144296/157046107-73fd3e1d-23d0-4450-85a7-16ee5265940d.gif)

## 참고문헌
- 개인 블로그(Tistory): [https://heytech.tistory.com/325](https://heytech.tistory.com/325)
- Gitgub: [https://github.com/park-gb/youtube-content-scaper](https://github.com/park-gb/youtube-content-scaper)

## 📝 License
```
MIT License

Copyright (c) 2022 Gyeongbin Park

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
