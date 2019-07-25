# How To Export & Convert From XML To CSV:

***

* iOS (iPhone) 및 watchOS (Apple Watch) 장치의 상태 및 건강 데이터가 포함 된 HealthKit XML 파일을 CSV 파일로 변환합니다. 
* [파이썬(My Heart Rate(bpm) For Time Series Analysis)을 이용](https://github.com/leehaesung/My_Heart_Rate_For_Time_Series_Analysis)하여 데이터를 플롯 및 데이터를 플롯 및 시계열 분석합니다.
* 이 프로젝트는 Python 버전 3을 사용합니다.

## Let's export.
* 첫 번째 단계는 iPhone에서 HealthKit 데이터를 얻는 것입니다.
  * Health 앱을 실행합니다.
  * 오른쪽 상단의 아이콘을 탭합니다.
  * 'Export Health Data'를 탭합니다.
  * [Convert_HealthKit_Data.py](https://github.com/leehaesung/My_Heart_Rate_For_Time_Series_Analysis/raw/master/02_Codes/Convert_HealthKit_Data.py) 다운로드하세요.

![HowToExportHealthKitData](https://raw.githubusercontent.com/leehaesung/My_Heart_Rate_For_Time_Series_Analysis/master/01_Images/HowToExportHealthKitData.png)

이렇게하면 'export.zip'아카이브가 제공됩니다. 이 파일을 컴퓨터로 전송하십시오. 압축을 푼 'apple_health_export'디렉토리에 'export_cda.xml'및 'export.xml'이 표시됩니다. 'export.xml'파일을 선택하십시오. 컴퓨터에 XML 파일이 있고, Python 3 이상이 설치되어 있으면 명령 행에서 다음을 수행하십시오.



```
python3 Convert_HealthKit_Data.py [Import file.xml] [Export file.csv]
```

* 예 :

```
python3 Convert_HealthKit_Data.py export.xml export.csv
```
