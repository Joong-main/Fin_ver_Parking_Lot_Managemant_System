# _Parking_Lot_Managemant_System (FIN_VER)

## 전화번호를 기본키(PRIMARY KEY)로 활용하여 주차 차량을 등록,삭제, 조회할 수 있으며, 관리자 권한을 통한 모든 정보 조회가 가능하다

## 프로그램 기능 설명 

<ul> 프로그램을 실행하면 UserInfo.txt 에서 값을 가져와 연결 리스트 노드에 추가한다. </ul>


<ol> 1.주차를 선택하면 노드를 생성하고 전화번호, 차량 번호를 입력 받아 등록 시점의 시간과 함께 노드에 저장한다. </ol>
</br>
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/1%EB%B2%88%EC%84%A0%ED%83%9D.PNG" ><img>

<ol> 2.출차를 선택하면 해당 전화번호를 키로 가지는 노드를 삭제한다. </ol>
</br>
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/2%EB%B2%88%EC%84%A0%ED%83%9D.PNG"></src>
<ol> 3.조회를 선택하면 기본키인 전화번호를 기준으로 노드를 탐색한다. </ol>
</br>
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/3%EB%B2%88%20%EC%84%A0%ED%83%9D.PNG"></src>
<ol> 4.관리자를 선택하면 패스워드 확인을 통해 패스워드가 일치할 경우에만 전체 차량, 고객 정보를 출력한다. </ol>
</br>
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/4%EB%B2%88%EC%84%A0%ED%83%9D.PNG"></src>
<ol> 5.종료를 선택하면 노드에 저장된 정보를 기반으로 파일을 작성하고 프로그램을 종료한다. </ol>
</br>
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/5%EB%B2%88%20%EC%84%A0%ED%83%9D.PNG"></src>

</br>
</br>
</br>
</br>

## 소스 코드 설명

* 연결리스트, 함수 선언
 <img src= "https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/1.%20%EC%97%B0%EA%B2%B0%EB%A6%AC%EC%8A%A4%ED%8A%B8%20%EB%B0%8F%20%ED%95%A8%EC%88%98%20%EC%84%A0%EC%96%B8.PNG" ></img>
 
 <ol>헤더 파일, 관리자 비밀번호와 연결리스트 구조를 정의 한다.</ol>
 <ol>메뉴창 프린트 함수, 노드의 생성, 삽입, 탐색, 삭제, 전체 출력, 파일쓰기의 주요 함수를 정의한다.</ol>
 
 
</br>
</br>
* print_menu 함수
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/5.%20%ED%94%84%EB%A6%B0%ED%8A%B8%20%EB%A9%94%EB%89%B4%ED%95%A8%EC%88%98.PNG"></img>

<ol>직사각형 디자인으로 선택 항목을 프린트 한다.</ol>

</br>
</br>

* 노드 생성함수
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/6.%20%EB%85%B8%EB%93%9C%EC%83%9D%EC%84%B1%ED%95%A8%EC%88%98.PNG"></img>
<ol> 새로운 노드를 생성하고 전화번호와 차량번호를 사용자로 부터 입력 받아 노드 멤버 변수에 추가한다.</ol>
<ol>return_time 함수를 인자로 사용하여 return 받은 현재 시간 정보 문자열을 노드 멤버 변수에 추가한다.</ol>
<ol>새로운 노드를 리턴한다.</ol>

</br>
</br>

* 노드 삽입함수
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/7.%20%EB%85%B8%EB%93%9C%EC%B6%94%EA%B0%80%ED%95%A8%EC%88%98.PNG"><img>

<ol>만약 기존에 연결리스트가 없다면 새로운 노드를 생성한다.</ol>
<ol>연결리스트에 노드있다면 ptr이 이동하여 마지막 주소를 찾고 마지막 연결리스트의 맨 끝에 노드를 연결한다.</ol>

</br>
</br>

* 노드 탐색 함수
<img src="https://github.com/Joong-main/Fin_ver_Parking_Lot_Managemant_System/blob/main/img/8.%EB%85%B8%EB%93%9C%20%ED%83%90%EC%83%89%ED%95%A8%EC%88%98.PNG"></img>

<ol>검색할 전화번호(기본키)를 입력받아 입력받은 전화번호와 노드의 멤보변수의 정보가 같을때 까지 이동한다</ol>
<ol>만일 같은 노드들의 멤버 변수중 같은 것이 있다면 그 노드의 주소를 리턴, 없으면 NULL을 리턴한다.</ol>




