# FrameLayout
FrameLayout 스터디


# 프로젝트 폴더에 이미지 추가하기
/app/res/drawable 폴더에 이미지 복사
이미지의 이름에는 영문 소문자, 숫자, _기호만 사용가능
영문 대문자 사용 불가, 이미지의 이름이 숫자로 시작 불가


# XML 레이아웃에서 설정한 id를 소스 코드에서 참조 할 수 있다.
XML 레이아웃 파일에서 id 값으로 "@+id/imageView"를 부여했다면 자바 소스 코드에서는 R.id.imageView라는 값으로 id를 참조할 수 있다.
즉, 다음과 같은 형식이다.
XML 레이아웃 파일에서 id 지정할 때 -> @+id/아이디
자바 소스 코드에서 참조할 때 -> R.id.아이디

# findViewByld 메서드의 의미 생각
하나의 화면은 XML 파일과 소스 파일로 나눠져있다. 이 두 개의 파일이 쌍을 이루면서 하나의 화면을 만든다.
어떤 XML 파일과 어떤 소스 파일이 하나의 쌍을 이루는지에 대한 정보는 소스 파일에 들어가 있다.
엑티비티 소스 파일에는 setContentView 라는 메서드가 있어서 파라미터로 XML 파일을 넘겨줄 수 있는데, 이 파라미터를 이용해 소스 파일과 XML 파일이 연결됨

이렇게 두 개의 파일이 쌍으로 연결되게 되면 소스 파일에서는 XML 파일에 들어 있는 뷰를 찾아 사용 가능
findViewByld 라는 메서드 이름은 ID를 이용해 뷰를 찾는다는 의미임.
XML 파일에 추가한 뷰에는 ID 값을 할당할 수 있다. 소스 파일에서는 그 ID를 이용해 메모리에 만들어진 뷰 객체를 찾을 수 있다.
