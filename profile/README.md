# Wattgam(Client)
서강대학교 2021-2학기 캡스톤디자인II 과목의 프로젝트의 일환으로 제작된 프로젝트입니다.  
[캡스톤디자인 위키 페이지 링크] http://cscp2.sogang.ac.kr/CSE4187/index.php/%EC%99%94%EB%8B%A4%EA%B0%90

</br>

## 왔다감 서비스 소개
AR 필터 카메라를 사용한 위치 기반 모바일 SNS입니다.


### Demo Video
https://youtu.be/nWbKHV_DNrU  

![image](https://user-images.githubusercontent.com/31800284/147137687-d1485e35-6848-4125-b1e0-d6a89546163f.png)
![image](https://user-images.githubusercontent.com/31800284/147137734-a670f503-33ff-400b-8edb-8a9a9e81e429.png)
![image](https://user-images.githubusercontent.com/31800284/147137739-baa20f46-4cae-44d0-85f1-4a8d5387a991.png)

### 게시글 작성
사용자는 특정 위치에서 AR 필터를 사용한 사진을 촬영하여, 다녀간 위치에 업로드할 수 있습니다. 이 때 현재 장소에 기반하여 게시물이 업로드되며, 간단한 글도 함께 작성할 수 있습니다.
</br>  
### 지도/게시글 열람
사용자의 현재 위치에 기반하여, 주변 1km * 1km 공간 안에 저장된 게시물을 불러옵니다. 해당 위치에 저장된 게시물의 수를 말풍선의 형태로 보여주며, 게시글이 10개 이상 쌓인 장소에는 10/20/30개에 따라 차등을 두어 랜드마크 아이콘이 말풍선과 함께 매핑됩니다. 말풍선을 터치하면 해당 위치에 저장된 게시물들을 확인할 수 있습니다.
</br>
### 유저 페이지
유저마다의 유저 페이지를 제공합니다. 유저 페이지에서는 프로필 사진, 이름, Bio, 그리고 업로드한 게시물의 목록을 확인할 수 있습니다. 조회중인 페이지가 유저 자신의 페이지일 경우 프로필 정보를 수정할 수 있습니다.

</br>
</br>

# Stack
![image](https://user-images.githubusercontent.com/31800284/147134963-1f2e7ad7-8f13-466a-88f9-114ff3b06cc7.png)
### 클라이언트
* React-Native 프레임워크를 사용하여 Android 환경 내에서 구현했습니다.
* Android 환경에서 작동하는 AR SDK인 AR Core를 사용하여 AR 카메라를 구현하였습니다. 이 때 AR 카메라는 Android Native 환경에서 개발하여,  카메라 Fragment를 패키지화 해 React-Native와 연동하였습니다.

### 백엔드
* Django를 사용해 서버를 구현하였습니다.
* MySQL을 사용해 데이터베이스를 구현하였습니다.
* 사진의 다운로드/업로드가 잦은 프로젝트이기 때문에 미디어 서버를 분리하였습니다.
* heroku를 이용해 테스트 서버를 구현하였습니다.
