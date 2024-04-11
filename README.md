# Visual Studio code(VScode)
* vs code 실행 시 가장 먼저 확인해야할 것!
* 왼쪽 탐색기가 당일 작업폴더로 연결되어 있는지 확인하기!
* (위) 안되있다면 -> 파일 -> 작업폴더 닫기 후 -> 폴더열기 다시 진행 !
# html 시작
* git, gitHub 개념공부
* `<태그>` 웹페이지에서 의미적인 정보를 가지는 대상 
## HTML5 버전선언 
* `<!doctype html>`
## HTML 구조태그
* html : 웹의 시작과 끝. 문서 자체 의미.
* head : 웹 문서의 정보, 제목 포함 
* meta : 웹 문서의 정보 기록 
* title : 웹 문서의 제목 (브라우저 상단 표시)
* body : 웹 문서 내용 (실제 대부분의 서비스가 들어가는 본문) 
## 구조태그 속성 
* `lang="ko"` html문서 언어 설정
* `charset="utf-8"`다국어 문자열 설정
* `description` 사이트 요약 설명 
* `keywords` 사이트 검색 키워드 설정 
## 속성 문법 
`<태그 속성="값" 속성="값"></태그>`
* 태그와 속성 사이 공백 
* 속성과 속성 사이 공백(속성 개수 제한 없음)
* 속성은 시작태그에만 작성하기!
## 구조태그의 `title` 작성방법
* 메인페이지 -> 사이트명
* 메인페이지 -> 사이트명 | 광고문구추가
* 서브페이지 -> 페이지명 | 사이트명 
* ex) 책이름-저자명 | 서점명
* ex) 판매아이템명 | 사이트명 
## h1~h6 제목태그(block tag)
* h1~h3태그는 meta keywords와 동일한 검색키워드로 활용된다. (대제목일 수록 높음)
* h4~h6 태그는 거의 사용하지 않는다. 
* h1은 사이트의 로고 및, 서브 페이지 제목에서 주로 사용한다. 
* h 제목의 1~6레벨은 순서대로 작성해야 한다. 
 ## 단락 p(block tag)
 * 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
 * 제목(h)태그 종류와는 형제 태그 관계로 사용해야 한다. 부모-자식 안됨
 ## 인라인태그 br, em, strong, del, s, sup,sub 
 * `br` : 블록 내 줄바꿈 태그
 * `em` : 블록 내 강조 태그, 주로 내용 태그(p) 등에서 자식으로 사용 
 * `strong` : 블록 내 경고용 강조 태그 (위와 특징 동일)
 * `del` : 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용 
 * `s` : 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용 (del 자주 사용)
 * `sup, sub` : 윗첨자 (sup) 아래첨자 (sub) 수학, 과학 등의 기호에 사용 
 ## 인용문 처리 blockquote, q
 * `blockquote(block)` : 단락 자체가 인용문에 해당할 때 사용, p태그와 부모-자식 관계로 사용해선 안된다!
 * `q(inline)` : 단락(p) 내에서 일부가 인용문에 해당할 때 사용 
 * 공통 속성 `cite="url"` : `blockquote`, `q`로 인용문 처리할 경우 출처 표시용도로 주소(url)을 담아주는 속성. 
 ## 특수문자 태그
 * <p>&copy; &reg;저작권 마크로 많이 쓰이는 특수문자태그</p>
 * `&` 시작 `;` 종료
 * `&copy` &시작과 copyright의 copy ; 종료
 ## 주소 태그
 * `address` : 연락처, 회사소개, 고객센터 등으로 사용
 * 다른 블록을 자식또는 자손으로 배치할 수 없고 footer영역에서 주로 사용
 ## 수평선 태그
 * `hr` :  사이트 각 영역을 구분할 때 사용
 * css에선 표현하지 않고 숨기는 경우가 대부분이며 주석과 같이 태그 구조 이해에 주 용도로 사용 
 ## 컴퓨터 명령어 태그
 * `code` : 컴퓨터가 지원하는 다양한 명령어를 화면에 표시할 경우에 사용 
 ## 링크 태그 a
 * block, inline 특징을 모두 가진다. 
 * 절대경로와 상대경로를 href 속성에 작성한다. 
 * 상대경로는 a태그 작성중인 파일 위치 기준 연결하고자 하는 목적지 파일이 같은 위치에 있는지, 하위 위치에 있는지, 상위 위치에 있는지에 따라 다르게 작성한다. 
 * ./ 현재 위치에서 시작
 * ../ 상위 폴더로 나가기 
 * `./doll.jpg` : 현재 위치에서 doll.jpg 파일 찾기
 * `../doll.jpg` : 상위 폴더로 한단계 나가서 doll.jpg 파일 찾기
 * `../a/doll.jpg` : 상위폴더로 한단계 나가고 a 폴더로 들어가서 doll.jpg 파일 찾기
 * `./b/doll.jpg` : 현재위치에서 b 폴더로 들어가서 doll.jpg 파일 찾기 
 ## 바로가기링크란?
 *  `<a href=”#id”>` : 태그가 가진 아이디명을 href 속성에 작성하여 바로가기 링크로 활용할 수 있습니다.  
 * 단순 페이지 이동이 아닌 특정 위치로 스크롤 이동하는 바로가기 기능 
 ## 바로가기 링크 제작 순서 및 주의사항
 * 바로가기 링크의 목적지에 id를 먼저 쓴 후 위에 바로가기 링크에 #을 붙이고 id를 써야합니다.
 * 1. 이동 목적지에 가장 가까운 태그에 `id` 적용하기
 * 2. 링크 대상에 `#id` href 속성값에 담기
 <!-- 주의 사항 -->
 * #은 아이디 이동 링크에만 사용하기 
  ## 파비콘 적용 순서
 * `<link rel=”#” href=”#” type=”image/x-icon”>` : 탭 및 작업표시줄 등에 웹을 구분가능하게 하는 아이콘을 파비콘이라고 합니다. 
 * png,jpg,gif 등의 이미지를 ico 확장자로 변환하여 사용할 수 있습니다. 
 * 16*16 ~ 180*180px 까지 웹/앱 환경에 따라 정사각형 비율로 제작하여 사용합니다. 
 * web favicon size : 16*16, 32*32, 96*96
 * apple favicon size : 57*57 ~180*180
 * android favicon size : 192*192
 * 1. 파비콘 크기로 이미지 다운받거나 편집하기 
 * 2. html에서 head 안에 link 태그로 `favicon` href주소 연결하기
 ## 이미지 태그 `img`(inline)
 * `<img> 태그` : src 이미지 경로 속성의 값으로는 상대경로 방식으로 작성하는 것을 권장합니다. 
 * 대체텍스트 alt 속성을 필수로 작성해야 합니다. 
 * 이미지 사용 시 의미전달이 필요한 이미지와 아닌 이미지를 구분해서 사용해야합니다.
 * `<img src=”url” alt=””>`필수
 * img 태그는 인라인태그이고 a 밖으로 나갈수 없음
 ## figure, figcaption 태그
 * 문서 안 사진을 감싸는 틀로서 활용하고 사진의 캡션을 정의할 수 있습니다. 
 ## video 태그
 * autoplay muted loop controls -> `autoplay`:자동재생 | `muted`:음소거 | `loop`:반복 | `controls`:통제 수단
 * 유튜브 영상의 소스를 복사 할 때 
 * 유튜브 제목`?autoplay=1&mute=1&loop=1` title=~~ 
 ## Class, id 많이 사용하는 키워드 
 * wrapper, wrap, area 전체 묶는 영역
 * contents, container 중~소 묶는 영역 
 * group, g 간단한 소그룹 영역 
 * top, btm, left, right 레이아웃 방향을 의미하는 키워드 
 * ex) 의미있는 단어_영역명 
 * 예시 : product_wrap, item_area, price_g, main_contents, top_btn
 ## div, span 그룹태그
 ### div 
 * 인라인과 블록이 2개 이상 형제일 경우 묶어주는 그룹태그
 * 레이아웃 기준 1행에 2열 이상 배치일 경우
 * 특정 의미를 가진 행에 같은 디자인 요소
 ### span
 * 인라인이 2개 이상 형제일 경우 묶는 그룹태그
 * 의미없는 디자인 요소 인라인 처리 필요 시 사용 
 ## html5 semantic tag
 ### header
 * 로고 및 내비게이션을 묶어주는 웹 사이트 레이아웃 태그입니다.
 * 제목, 로고, 검색 폼, 작성자 이름 등의 요소도 포함할 수 있습니다.
 ### nav
 * 로고 및 웹사이트 주요 내비게이션을 묶어주는 웹 사이트 레이아웃 태그입니다.
 * 다른 페이지로의 링크를 보여주는 구획을 나타냅니다. 자주 쓰이는 예제는 메뉴, 목차, 색인입니다.
 ### gnb, inb, snb
 * `gnb(global navigation bar)` - nav 묶이는 대상
 * `lnb(local navigation bar)`
 * `snb(side navigation bar)`
 ## ul, ol, li
 * `ul` : 순서가 없는 목록 
 * 2개 이상의 목록(li) 구조를 묶어주는 그룹태그(ul)
 * 목록의 순서와 연관없을 경우 ul만 사용합니다. 
 * `ol` : 순서가 있는 목록
 * 2개 이상의 목록 (li)구조를 묶어주는 그룹태그(ol)
 * 목록의 순서가 있을 경우 ol만 사용해야한다.
 * 그룹은 반드시 목록의 가장 근접한 부모로써 존재해야합니다. 
 * `ol`,`ul`의 자식은 무조건적으로 li여야한다. 
 ## details, summary
 * `details` : "열림"상태일 때만 내부정보를 보여주는 정보 공개 위젯을 생성합니다. (요약부분을 펼쳐보게 할 수 있는 역할)
 *  `summary` : details의 자식요소로 요약이나 레이블을 제공할 수 있음
 ## footer, mark, main, time
 * `footer` : 웹페이지 가장 하단에 위치한다. 구획의 작성자, 저작권 정보, 관련 문서 등의 내용을 담고 있다.
 * `mark` : 현재 맥락에 관련이 깊거나 중요해 표시 또는 하이라이트한 부분을 나타낸다. (형광팬으로 칠 한 것 처럼 하이라이트처리 해줌) 
 * `main` : 문서<body>의 주요 콘텐츠를 나타냄, 주요 콘텐츠 영역은 문서의 핵심 주제나 앱의 핵심 기능에 직접적으로 연결됐거나 확장하는 콘텐츠로 이루어짐 
 * `time` : 일반 텍스트로 보이는 날짜와 시간정보를 진짜 날짜, 시간 정보임을 html에게 알려주기 위해 사용된다. 