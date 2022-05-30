

## Play List ▶️
JPA를 이용해 음원 DB 테이블 구성, 데이터 저장, 수정, 삭제하는  API 구현

## Team members 👩‍👩‍👦‍👦

-   배서현 (GitHub Url :  [https://github.com/Do-it-chu](https://github.com/95Glory))  
-   문선화 (GitHub Url :  https://github.com/woowsnu)  
-   김현진 (GitHub Url :  [https://github.com/Hyeonjin-ee](https://github.com/95Glory))  
-   김영광 (GitHub Url :  [https://github.com/95Glory](https://github.com/yunjo1))  

## Tech Stack
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">  <img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">   <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white">   

## Domain🛠️
**[Album Entity]**
* int album_id : 앨범 아이디(**PK**)
* String albumTitle : 앨범 제목
* String artist : 앨범 아티스트  
* String albumGenre : 앨범 장르
* LocalDate releaseDate : 앨범발매일

**[PlayList Entity]**
* int playListId ; 플레이리스트 고유 아이디(**PK**)
* String playlistName ; 플레이리스트명

**[PlayList Entity]**

* int playListSongId ; 플레이리스트음원 아이디(**PK**)
* List<Album> album ; 앨범 아이디
* List<Song> song ; 음원 아이디
* Playlist pl ; 플레이리스트 아이디

**[Song Entity]**
* int songId ; 음원 고유 아이디(**PK**)
* String title ; 음원 제목
* String artist ; 음원 가수
* String length ; 음원 음원길이	
* Album album ;  앨범 앨범(**FK**)


## Requirements 🤔

☝️ 앨범, 음원 데이터 등록  

✌️ 앨범 아이디로 음원 조회

👌  플레이리스트 생성

🖖 플레이리스트 이름 수정

🖐️ 플레이리스트에 음원 추가

##   구현 예제



## Trouble Shooting
- 처음 구현하려고 했던 기능은 음원 사이트에서 사용하는 플레이리스트처럼 플레이리스트를 생성하고 플레이리스트 안에 음원을 넣고, 장르별로 구분하여 조회 및 CRUD 구현을 하고자 했으나 아래 기능들은 에러 발생으로 구현하지 못하였음
-   
### Model(PlaylistSong)
  (사진)
  - 다량의 조인, 매핑에 대한 에러가 발생해 엔티티 테이블 자체가 생성되지 않는 오류가 지속적으로 발생하여 프로젝트 마무리를 위해 구현했던 연관관계, 조인 설정을 모두 삭제하고 진행함.
  
### Path(/song)
- jqpl 문법 사용해 등록된 전체 곡을 조회하고 싶었으나 하나의 곡만 조회되는 현상 발생

### Path(/songInAlbum)
- jqpl 문법 하나의 앨범에 들어있는 전체 곡을 조회하고 싶었으나 하나의 곡만 조회되는 현상 발생

## Review  
### 배서현  
---  

### 문선화  
---  
  

### 김현진 
배운 내용을 실제로 적용하는 과정은 언제나 어려운 것 같다. 
특히, 이번 프로젝트에서 테이블 간에 관계를 정의하고 맵핑하는 과정은 이해도 어렵고 너무 많은 오류가 나서
더더욱 힘들었다. 처음에 기획했던 기능들을 모두 구현하지는 못했지만, 배운 걸 복습하고 응용하면서 많은 걸 배울 수 있는 좋은 시간이 되었던 것 같다.

---  
 
### 김영광  

프로젝트를 할 때마다 다음 나갈 진도는 최대한 이해를 하여 팀원들에게 피해를 안끼쳐야지 다짐하였건만, 이번에는 코드 구현을 완전히 하지 못하였다. 이번 프로젝트를 하면서 자신에게 실망하고 아쉬웠지만 그래도 팀원들과의 화합으로 인해 100프로의 완성도는 아니였지만 멋있는 프로젝트에 내 이름을 올릴수 있다는것에 팀원들에게 너무 고맙다.

---  
  

