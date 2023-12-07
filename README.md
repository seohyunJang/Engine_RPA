# Engine_RPA
: (HHI) Engine RPA 

# Version
  - Param_update_v5 (2023/09/19)  
    : input xlsx 파일 내의 sheet에 따라 새로운 폴더 생성, 각 폴더에 Ref case 폴더 내의 파일 복사, 이 중 spray.in 파일의 정보만 해당 sheet 정보에 따라 수정
  - Param_update_v5_spray (2023/12/06)  
    : input xlsx 파일 이름의 새로운 폴더 생성, Ref case 폴더 내의 파일 복사, xlsx 폴더 sheet 정보에 따라 spray_case{i}.in 형태로 복수의 spray.in 파일 생성

# How to Use?
## 1. Engine Parameter auto-transition
  - Prerequisite :  
      실행파일 (.exe)
      Ref case 폴더 (함께 복사해야 할 파일 리스트 - 내부에 spray.in 파일 必, exe 시랭파일과 같은 경로상에 위치)
      input file 폴더 (spray.in 파일 기준, 파라미터 변경값을 포함한 xlsx 파일 존재)
      output file 폴더 
    
  - 실행방법 :  
      1. exe 파일 실행 (일정 시간 기다림 필요, 화면이 안 뜰 때 Enter 입력)
      2. 가이드에 따라 input file 경로 입력 (파일 탐색기 주소 Ctrl+C, Ctrl+V)
      3. 가이드에 따라 output file 경로 입력 (파일 탐색기 주소 Ctrl+C, Ctrl+V)
      4. sheet에 따라 자동 처리, 결과물 output
   
# Caution!
  - 실행파일과 Ref case 폴더는 같은 경로상에 위치!
  - 파라미터 변경 정보를 포함한 xlsx 파일의 sheet 이름은  
    (Param_update_v5) param{i}, i는 int Ex) param1, param10, param99
    (Param_update_v5_spray) case{i}, i는 int Ex) case1, case10, case99
