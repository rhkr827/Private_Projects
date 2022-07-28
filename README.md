[English Version](README_ENG.md)

# 1. Ovalis_Log_Analyzer - Private

- Software Solution Log 분석 툴
- 개인 업무 자동화 프로그램

#### 목적

- 반도체 공정 분석 솔루션 유지 보수 업무 담당
  - SW Patch와 Server, DB 상태 및 솔루션 정상 동작 여부 등 모니터링 업무
  - 해당 솔루션은 독일 Qoniac사의 Ovalis이며 현재 KLA에 합병
  - Windows Server와 MSSQL로 구성된 시스템
- 솔루션 Log 분석이 필요한 경우, 엑셀의 텍스트 나누기 기능으로 차트화하여 상태 확인 및 보고 업무
- 반복 작업을 자동화하는 방법을 찾다가 구글링과 함께 프로그램 제작

#### 기능

- 전체 또는 90일의 Data별 Trend 차트로 서버별 시스템 상태 확인 기능
  - 항목으로는 DB Size, CPU, Memory 변화량, 기능별 계산 소요시간 및 사용 시간, 사용 유저 수, 발생 에러 Log 등
- Daily Log는 더 세부적인 Data display와 분석 기능

##### 개발 환경

- IDE : Visual Studio 2015 Community(Visual Studio 2019 Comminity로 변경)
- UI : WinForms
- Function : C#
- Database : SQLite
- Framework : .NET Framework 4.5.2

# 2. FSR_Analyzer - Private

- 공수 관련 통계 프로그램 개발
- 개인 업무 자동화 프로그램

#### 목적

- 당시 회사내 엑셀 파일로 작성하고 수작업으로 통계 계산하여 제출
- ERP 도입 후 엑셀에서 웹으로만 변경되었지, 통계 계산 작업은 여전히 수작업
- 귀차니즘으로 인해 독학으로 Googling과 함께 공수 통계 프로그램 제작

#### 기능

- 당시 회사 엑셀 포멧과 ERP에서 다운로드한 엑셀 Format Parsing 및 DB화
- UI에서 주, 월, 년도별로 업무시간 통계치를 표로 표시.
- Excel로 통계 Export 기능(보고용)

##### 개발 환경

- IDE : Visual Studio 2015 Community(Visual Studio 2019 Comminity로 변경)
- UI : WinForms
- Function : C#
- Database : SQLite
- Framework : .NET Framework 4.5.2

# 3. MyMoney_CSharp_WinForms - Private

- 가계부 프로그램(1st version)
- DB 및 SQL 공부 및 취미로 제작한 프로그램

#### 목적

- DB 관련 업무를 하며 DB/SQL에 대한 흥미가 생겨 개인 공부 시작
- Database 관련 공부에 필요한 Sample Data로 거래내역를 선택
- 구글링과 함께 거래내역 통계를 보여주는 프로그램 제작

#### 기능

- DB Import
  - 은행별, 증권사별, 카드사별 거래내역 홈페이지에서 Excel형식으로 다운로드 및 Paring 후 DB Importing
  - 추가로 통장이 있는 경우는 수작업으로 입력, Excel로 가계부 작성한 기간은 별도 Parsing 및 DB Import
- UI
  - Table 형식으로 월별 총수입/지출을 보여주는 Page
  - Table 형식으로 거래내역을 보여주는 Page(Filter 기능 없음)
  - 최종적으로는 미완성. 회사 내 업무 관련 공부 목적으로 새로운 버전 제작 계획으로 UI 제작 중단

#### 개발 환경

- IDE : Visual Studio 2017 Community(Visual Studio 2019 Community으로 변경)
- UI : WinForms
- Function : C#
- Database : SQLite
- Framework : .NET Framework 4.5.2

# 4. MyMoney_CSharp_WPF

- 가계부 프로그램(2nd version)
- 취미로 제작한 프로그램

#### 기능

- DB importing
  - Openbank 서비스는 제공하는 뱅크샐러드 data를 DB Import
  - 초기 뱅크샐러드 Web에서도 거래내역 볼수 있어, 해당 page의 html parsing 후 DB importing
  - 이후 Web service 중단 후, App의 Excel Export 기능(암호화)으로 Gmail로 전송
  - 최종적으로 Google Gmail API 사용하여 첨부파일 다운 및 Parsing 후 DB importing
  - 현재, 처음 아르바이트 했던 2006년부터 현재까지 모든 거래내역 DB화. 계속 위 방식으로 업데이트 중
- UI
  - 기간별 총수입, 총지출, 소비카테고리별 지출내역 등의 Data를 Chart로 볼 수 있도록 Dashboard 페이지
  - Filter 기능 추가된 거래내역 Table 페이지
  - DB importing 기능을 사용하는 업데이트 페이지
  - UI 만들다가 중단. 프로그래밍이 취미에서 직업이 되다보니 자연스럽게 중단

#### 개발 환경

- IDE : Visual Studio 2019 Community
- UI : WPF(DevExpress)
- Function : C#
- Database : Microsoft SQL Server 2017
- Framework : .NET Framework 4.5.2, Entity Framework 6
- API : Google API OAuth, Gmail API
