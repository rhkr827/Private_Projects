[한국어 버전](README.md)

# 1. Ovalis_Log_Analyzer - Private

- Software Solution Log Analysis tool
- Personal program for automation tasks

#### Goals

- Maintenance Processing and Control Solution in semiconductor manufacturing processing
  - My role was patching SW and monitoring server and DB status and if the solution was normal operating or not
  - The solution called Ovalis(Qoniac, Current merged with KLA) configuring Windows Server and MS-SQL
- When analyzing solution log, usually using excel fuction split by text and made chart for checking status and reporting
- To avoid repetitive tasks, this tool developed with googling

#### Function

- Display trend charts Whole or 90 days period, possible checking system status per server
  - parameters are DB Size, CPU and Memory usage, elapsed time and usage time per functions of Ovalis, a number of users, errors etc.
- In case daily log, possible more detailed analyzing the solution system

#### Development environment

- IDE : Visual Studio 2015 Community(Converted to Visual Studio 2019 Community)
- UI : WinForms
- Function : C#
- Database : SQLite
- Framework : .NET Framework 4.5.2

# 2. FSR_Analyzer - Private

- Developed program for statistics of working time
- Personal program for automation tasks

#### Goals

- Writing working time in Excel and calulate statistics manually for reporting
- After applied ERP System, but still calculate manually
- Due to annoying the repeated task, started to develop the program with googling

#### Function

- Parsing and importing to DB from Excels old format and downloaded from ERP
- In UI, possible to check working time statistics per week, month and year
- Function for Export Excel to reporting

#### Development environment

- IDE : Visual Studio 2015 Community(Converted to Visual Studio 2019 Community)
- UI : WinForms
- Function : C#
- Database : SQLite
- Framework : .NET Framework 4.5.2

# 3. MyMoney_CSharp_WinForms - Private

- A program for my financial ledger(1st version)
- Developed program for studying DB and SQL as hobby

#### Goals

- Started to study individually because I became interested in DB/SQL while working on DB
- Selected my banck transactions as sample data for studying Database.
- Developed program fucntion for importing to DB and UI with googling

#### Functions

- DB import
  - Downloding my transactions by Excel format from per banks, securities firm and credit card company
  - Additionally typing manually from bankbook or parsing excel I had wrote finanacial ledger and DB importing
- UI
  - A page for dashboard such as total income/expense per month via table
  - A page for table to show transaction but no filters
  - Stopped creating UI due to having new plan to develop new version of program to practice for my role in company

#### Development environment

- IDE : Visual Studio 2017 Community(Converted to Visual Studio 2019 Community)
- UI : WinForms
- Function : C#
- Database : SQLite
- Framework : .NET Framework 4.5.2

# 4. MyMoney_CSharp_WPF

- A program for my financial ledger(2nd version)
- Developed program as hobby

#### Functions

- DB importing
  - Imported my transactions using App data called Banksalad support Openbank service
  - Begining, imported parsing Banksalad web page(html)
  - Afterwards, stopped web service, and using new service exported Excel(encrypted) and sent to Gmail
  - Finally, using Google Gmail API, downloading attachments and parsing then import to DB
  - Now, all transactions were imported to DB since 2006 when I worked part-time for the firt time
- UI
  - A page for dashboard such as total income/expense per period and expense per categories via charts
  - A page for table to show transaction with filters
  - A page for update data by DB importing function
  - Couldn't finished creating UI
  - The reaseon is progrming had changed just hobby to a job as SW Developer

#### Development environment

- IDE : Visual Studio 2019 Community
- UI : WPF(DevExpress)
- Function : C#
- Database : Microsoft SQL Server 2017
- Framework : .NET Framework 4.5.2, Entity Framework 6
- API : Google API OAuth, Gmail API
