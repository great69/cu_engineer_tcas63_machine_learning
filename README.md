# วิเคราะห์คะแนนต่ำสุด วิศวะ จุฬา TCAS63 รอบ 3
_by พี่เกรท ออนดีมานด์_

ในโปรเจกนี้ เราจะใช้ Machine Learning Model มาทำนายคะแนนต่ำสุดสอบติดคณะวิศวกรรมศาสตร์ จุฬาลงกรณ์มหาวิทยาลัย ในระบบการคัดเลือก TCAS รอบที่ 3 ของปีการศึกษา 2563 โดยใช้ข้อมูลสถิติคะแนน GAT/PAT ของ สทศ. ในปี 2555-2562

## Install
โปรเจกนี้ต้องใช้ **Python 3.x** และลง Python libraries ต่อไปนี้:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [ScikitLearn](https://scikit-learn.org/)

และจำเป็นต้องลงโปรแกรมสำหรับเปิด iPython Notebook [iPython Notebook](http://ipython.org/notebook.html)

แนะนำให้ลง [Anaconda](https://www.continuum.io/downloads) ซึ่งเป็น Python Package ที่มี libraries ที่ต้องใช้ครบในตัวเอง

## Files
- `tcas3_eng_cu_analysis_2563_draft_06.ipynb` : Notebook ที่ใช้วิเคราะห์ข้อมูล
- `engcuraw63_04.csv` : สถิติคะแนน GAT/PAT ปี 2555-2563 และคะแนนต่ำสุดที่สอบติดวิศวะจุฬารอบรับตรงในปี 2555-2562

## Run
ใน terminal หรือ command window, ให้ navigate ไปที่ project directory (ที่มีไฟล์ README นี้) และรัน commands ต่อไปนี้:

```bash
ipython notebook Project_Image_Classifier_Project.ipynb
```  
or
```bash
jupyter notebook Project_Image_Classifier_Project.ipynb
```

## Data
ข้อมูลดิบมาจากเว็บไซท์ของ [สทศ.](https://www.niets.or.th/th/) และในปีเก่าๆ ที่ไม่มีในเว็บไซท์แล้ว หาจากการเสิช google ด้วย keyword `สถิติ GATPAT (ปีการศึกษา)` ซึ่งบางข้อมูลเป็นไฟล์รูปในเว็บบอร์ด จึงไม่สามารถอ้างอิงได้ในที่นี้

และสถิติคะแนนต่ำสุดที่สอบติดวิศวะฯ จุฬา ปี 2555-2562 หาได้จากการเสิช google ด้วย keyword `คะแนนต่ำสุด รับตรง วิศว จุฬา (ปีการศึกษา)`

## Disclaimer
การวิเคราะห์นี้ ทำด้วยข้อมูลเท่าที่หาได้จากเว็บไซต์ สทศ. ซึ่งมีข้อมูลย้อนหลังถึงปี 2553 ที่เริ่มมีการสอบ GAT/PAT อีกทั้งเราไม่เอาคะแนนปี 53-54 มาคิดเพราะเกณฑ์การรับมี GPAX ด้วย ต่างจากปี 55 เป็นต้นไป ที่ใช้คะแนน GAT/PAT เพียงอย่างเดียว ดังนั้น จำนวนจุดของข้อมูลจึงมีจำกัดมากๆ อาจทำให้คะแนนที่ทำนายออกมา มีความแม่นยำที่ลดลง อย่างไรก็ตาม พี่จะทำนายแล้วระบุความคลาดเคลื่อนเอาไว้ให้ด้วยครับ
