# Sidebar Enhancements
- 사이드바의 기능을 향상시켜주는 패키지

참고 https://github.com/titoBouzout/SideBarEnhancements

# f12
- F12 키를 사용하면 브라우저에서 현재 파일을 열 수 있습니다.
- 절대 경로 사용 "Project -> Edit Projects Preview URLs"
```
{
	"S:/www/domain.tld":{
		"url_testing":"http://testing",
		"url_production":"http://domain.tld"
	}
}
```
- url_testing : F12를 통해 열리는 로컬 서버의 URL을 설정할 수 있습니다.
- url_production : ALT+F12를 통해 열리는 프로덕션 서버의 URL을 설정할 수 있습니다.
```
{
	"C:\dev\jquery.js.":{
		"url_testing":"http://dev.open.org",
		"url_production":"http://open.org/jquery.js"
	}
}
```
- dev 폴더의 jquery 파일을 로컬서버(f12)와 실제서버(alt+12) url로 각각 열 수 있다.
