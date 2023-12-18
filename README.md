
# Engine_RPA
: (HHI) Engine RPA 

# Version
  - Param_update_v5 (2023/09/19)  
    : input xlsx 파일 내의 sheet에 따라 새로운 폴더 생성, 각 폴더에 Ref case 폴더 내의 파일 복사, 이 중 spray.in 파일의 정보만 해당 sheet 정보에 따라 수정
    
  - Param_update_v5_spray (2023/12/06)  
    : input xlsx 파일 이름의 새로운 폴더 생성, Ref case 폴더 내의 파일 복사, xlsx 폴더 sheet 정보에 따라 spray_case{i}.in 형태로 복수의 spray.in 파일 생성

  - Param_update_v6 (2023/12/18)
    : input xlsx 파일 내 'Doe(final)' 시트의 정보에 따라 다수의 case 파일 생성 (Ref Case내 파일 복사, spray.in과 RateShape.in 파일 변경)

# How to Use?
## 1. Engine Parameter auto-transition
  - Prerequisite :  
![image](https://github.com/seohyunJang/Engine_RPA/assets/48125526/66d848cd-e1f7-45c6-b340-1ce0c718090f)


  - 실행방법 :  
      1. exe 파일 실행 (일정 시간 기다림 필요, 화면이 안 뜰 때 Enter 입력)
      2. 가이드에 따라 input file 경로 입력 (파일 탐색기 주소 Ctrl+C, Ctrl+V)
      3. 가이드에 따라 output file 경로 입력 (파일 탐색기 주소 Ctrl+C, Ctrl+V)
      (4. 가이드에 따라 RateShape 파일들을 포함한 경로 입력 (파일 탐색기 주소 Ctrl+C, Ctrl+V) -- Param_update_V6에 해당) 
      5. sheet에 따라 자동 처리, 결과물 output
   
# Caution!
  - Ref case의 spray.in 파일을 기준으로 설계되었기 때문에, 해당 파일이 바뀌면 안됨!
  - 실행파일과 Ref case 폴더는 같은 경로상에 위치!
  - 파라미터 변경 정보를 포함한 xlsx 파일의 sheet 이름은  
    (Param_update_v5) param{i}, i는 int Ex) param1, param10, param99
    (Param_update_v5_spray, Param_update_v6) case{i}, i는 int Ex) case1, case10, case99

# File Location  
  (보안상 관련 폴더는 EFAM 공유 폴더 내에 위치해있습니다)  
  *Z:\시스템성능연구실\9_개인폴더\장서현\대형RPA\[RPA]Param_update*

