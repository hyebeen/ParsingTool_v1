**인프라 취약점 진단 결과 파싱 도구
**

- 스크립트 결과(텍스트 파일) 파싱



V1
- 취약/양호 여부 판별 선택
- 위에 코멘트 처리 선택
  Ex) [진단 결과]
- 엑셀 결과 양식 : 서버 개수에 따라 열 추가
- 자동 인코딩(utf-8) 변환
  
  
  
V2
- V1에 비해 간소화
- 엑셀 결과 양식 : 서버 개수에 따라 행 추가
- 자동 인코딩(utf-8) 변환



사용법
1) 스크립트 결과(텍스트 파일)만 모아놓은 폴더 생성(폴더 내 파싱 도구 있으면 안됨.)
2) 파싱 도구 실행
3) 시작 패턴 및 마지막 패턴 입력
4) 필요에 따라 취약/양호 여부 판별, 코멘트 추가(V1만 해당)
5) 파싱 도구가 있는 디렉터리 내 엑셀 파일 생성



주의사항
1) 엑셀 파일이 생성된 이후 파싱 도구를 재실행하면 자동으로 기존 파일이 삭제될 수 있으니 주의
2) DRM 걸린 문서의 경우 파싱 도구가 돌아가지 않음
3) 상황에 따라 가끔 파싱 도구가 바로 종료되어 버리는 경우가 있음
   - 파싱 도구에서 자동 인코딩(utf-8)변환 해주기 때문에 메모장으로 열면 "utf-8"로 변환되어 있는 것을 확인할 수 있으나 이는 겉으로만 인코딩 된 경우가 있음. 이럴 때는 파싱 도구를 돌리기 전에 수동으로 "utf-8"로 변환해주어야 함. 메모장 > 다른이름으로 저장 > 인코딩(UTF-8) > 저장
