# 인프라 취약점 진단 결과 파싱 도구 #
![image](https://user-images.githubusercontent.com/17823031/123910354-467f7c00-d9b5-11eb-970f-f125fd2b41a1.png)
- 스크립트 결과(텍스트 파일)를 엑셀파일로 항목별 파싱   
   
-----------------------------------------
   
## V1 ##
- 취약/양호 여부 판별 선택
- 위에 코멘트 처리 선택
  Ex) [진단 결과]
- 자동 인코딩(utf-8) 변환   

### V1 결과 양식 ###
![image](https://user-images.githubusercontent.com/17823031/123603885-45bfdc00-d835-11eb-8d9d-68c55f5d90d5.png)
- 서버 개수에 따라 열 추가   

### V1 사용법 ###
1) 스크립트 결과(텍스트 파일)만 모아놓은 폴더 생성(폴더 내 파싱 도구 존재하지 않도록 주의)
2) 파싱 도구 실행
3) 시작 패턴 및 마지막 패턴 입력
    ```Ex) ####START###```
4) 필요에 따라 취약/양호 여부 판별, 코멘트 추가(V1만 해당)
5) 파싱 도구가 있는 디렉터리 내 엑셀 파일 생성  
6) 엑셀 파일에 항목 번호, 항목 명 복사하여 사용
   
-----------------------------------------
   
## V2 ##
- V1에 비해 간소화, **V2사용 권장**
- 자동 인코딩(utf-8) 변환   

### V2 결과 양식 ###
![image](https://user-images.githubusercontent.com/17823031/123909918-b2adb000-d9b4-11eb-911c-adca2a0ad1e6.png)
- 서버 개수에 따라 행 추가   

### V2 사용법 ###
1) 스크립트 결과(텍스트 파일)만 모아놓은 폴더 생성(폴더 내 파싱 도구 존재하지 않도록 주의)
2) 파싱 도구 실행
3) 시작 패턴 및 마지막 패턴 입력
    ```Ex) ####START###```
4) 파싱 도구가 있는 디렉터리 내 엑셀 파일 생성  
5) OS, IP 정보는 스크립트 결과(텍스트 파일)이름을 그대로 따오도록 하였으므로 필요 시 바꾸기(ctrl+h)를 통해서 변경하거나 불필요 시 삭제 -> 추후 보완 예정
6) 엑셀 파일에 항목 번호, 항목 명 복사하여 사용   
   
-----------------------------------------
   
## 주의사항 ##
1) 엑셀 파일이 생성된 이후 파싱 도구를 재실행하면 자동으로 기존 파일이 삭제될 수 있으니 주의
2) DRM 걸린 문서의 경우 파싱 도구 실행 불가
**3) 상황에 따라 가끔 파싱 도구가 바로 종료되어 버리는 경우
   - 파싱 도구에서 자동 인코딩(utf-8)변환 해주기 때문에 메모장으로 열면 "utf-8"로 변환되어 있는 것을 확인할 수 있으나 이는 겉으로만 인코딩 된 경우가 있음. 이럴 때는 파싱 도구를 돌리기 전에 수동으로 하나하나 "utf-8"로 변환필요 (*중요*)**
   ```'메모장 > 다른이름으로 저장 > 인코딩(UTF-8) > 저장' ```
4) 스크립트 내 시작 패턴 및 마지막 패턴이 나오지 않는 경우 파싱 도구가 돌아가긴 하나 엑셀파일 결과 내 항목이 밀려서 나올 수 있으므로 스크립트 전달 전 확인하여 스크립트 수정 필요
5) 메일로 전달 시 악성코드 탐지되는 경우 : 7zip으로 패스워드 걸어서 .7zip으로 압축한 후 .ogg로 확장자명 변경하여 전달
