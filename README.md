# Personality Prediction: Introvert vs. Extrovert Analysis
This project analyzes behavioral patterns to classify personality types (Introvert/Extrovert) using Data Analytics and Machine Learning techniques.
1. Dataset Overview
- The dataset consists of 2,900 samples with 7 key behavioral features:
- Time_spent_Alone: Time spent in solitude.
- Stage_fear: Anxiety regarding public performance or speaking (Yes/No).
- Social_event_attendance: Frequency of attending social gatherings.
- Going_outside: Frequency of leaving the house.
- Drained_after_socializing: Feeling of exhaustion following social interaction (Yes/No).
- Friends_circle_size: The total number of people in one's social circle.
- Post_frequency: Frequency of social media posting.

 2. Data Preprocessing
- To ensure model accuracy, the data underwent the following cleaning steps:
- Handling Missing Values: Missing numerical values were imputed using the Mean, while categorical values were replaced with the Mode.
- Feature Encoding: Qualitative data was converted into numerical format:
- Introvert → 0, Extrovert → 1.
- Yes → 1, No → 0.

3. Exploratory Data Analysis (EDA)
Key insights derived from data visualizations include:
- Social Media Engagement: Introverts show high density in low posting frequencies (0–2 times), whereas Extroverts exhibit a wider variety of posting behaviors (3–10 times).
- Key Drivers: Drained_after_socializing and Stage_fear showed a strong negative correlation with Extroversion (~ -0.85).
- Social Circle: Friend circle size is positively correlated with being an Extrovert (0.69) and significantly impacts social media engagement.

4. Machine Learning Model
- Logistic Regression was selected for its high interpretability and accuracy with this specific dataset:
- Train-Test Split: The data was divided into 80% for training and 20% for testing.
- Performance: The model accurately predicts personality types based on behavioral factors that align with real-world patterns.

5. Conclusion
- Personality is not just a subjective feeling but is reflected in measurable behaviors. In the digital age, Social Media Engagement and Social Circle Size have emerged as critical indicators that clearly distinguish Introverts from Extroverts.



โปรเจกต์วิเคราะห์พฤติกรรมเพื่อจำแนกบุคลิกภาพ (Introvert/Extrovert) โดยใช้เทคนิคการวิเคราะห์ข้อมูลและ Machine Learning
1. เกี่ยวกับชุดข้อมูล (Dataset Overview)
ชุดข้อมูลนี้ประกอบด้วยกลุ่มตัวอย่างจำนวน 2,900 แถว โดยมีตัวแปรที่ใช้ศึกษาพฤติกรรมทั้งหมด 7 ปัจจัยหลัก:
- Time_spent_Alone: เวลาที่ใช้คนเดียว
- Stage_fear: ความกลัวในการแสดงออก (Yes/No)
- Social_event_attendance: ความถี่การเข้าร่วมงานสังคม
- Going_outside: ความถี่ในการออกไปข้างนอก
- Drained_after_socializing: ความรู้สึกเหนื่อยล้าหลังเข้าสังคม (Yes/No)
- Friends_circle_size: ขนาดกลุ่มเพื่อน
- Post_frequency: ความถี่ในการโพสต์โซเชียลมีเดีย

2. การเตรียมข้อมูล (Data Preprocessing)
เพื่อให้โมเดลทำงานได้อย่างแม่นยำ ได้มีการทำความสะอาดข้อมูลดังนี้:
- Handling Missing Values: ตรวจพบค่าว่างในหลายคอลัมน์ จึงใช้วิธีแทนที่ด้วย Mean (ค่าเฉลี่ย) สำหรับข้อมูลตัวเลข และ Mode (ฐานนิยม) สำหรับข้อมูลหมวดหมู่.
- Feature Encoding: แปลงข้อมูลเชิงคุณภาพให้เป็นตัวเลข:
Introvert → 0, Extrovert → 1
Yes → 1, No → 0

3. การวิเคราะห์ข้อมูลเชิงสำรวจ (Exploratory Data Analysis - EDA)
จากการวิเคราะห์ผ่านกราฟ (Visualizations) พบ Insight ที่น่าสนใจดังนี้:
- Social Media Engagement: กลุ่ม Introvert มีพฤติกรรมการโพสต์ที่เกาะกลุ่มหนาแน่น (High Density) ในระดับต่ำ (0-2 ครั้ง) ขณะที่กลุ่ม Extrovert มีความหลากหลายในการโพสต์มากกว่า (3-10 ครั้ง)
- Key Drivers: พบว่าความรู้สึกเหนื่อยล้าหลังเข้าสังคม (Drained_after_socializing) และความกลัวเวที (Stage_fear) มีความสัมพันธ์เชิงลบกับความเป็น Extrovert อย่างรุนแรง (Correlation ~ -0.85).
- Social Circle: ขนาดกลุ่มเพื่อนมีความสัมพันธ์เชิงบวกกับการเป็น Extrovert (0.69) และส่งผลต่อความถี่ในการโพสต์โซเชียลอย่างมีนัยสำคัญ.

4. โมเดลการทำนาย (Machine Learning Model)
ได้เลือกใช้ Logistic Regression เป็นโมเดลหลักในการจำแนกประเภท เนื่องจากให้ผลลัพธ์ที่ตีความง่ายและมีความแม่นยำสูงกับข้อมูลชุดนี้:
- Train-Test Split: แบ่งข้อมูลเป็น 80% สำหรับสอนโมเดล และ 20% สำหรับทดสอบ.
- Performance: โมเดลสามารถทำนายบุคลิกภาพได้อย่างแม่นยำ โดยพิจารณาจากค่าความสัมพันธ์ของปัจจัยต่างๆ ที่สอดคล้องกับพฤติกรรมจริง

5. สรุปผลการวิเคราะห์ (Conclusion)
- บุคลิกภาพ (Personality) ไม่ได้เป็นเพียงแค่ความรู้สึก แต่สะท้อนออกมาผ่านพฤติกรรมที่วัดผลได้จริง โดยเฉพาะในยุคดิจิทัลที่ Social Media Engagement และ Social Circle Size กลายเป็นตัวชี้วัดสำคัญที่แยกแยะระหว่างคนกลุ่ม Introvert และ Extrovert ได้อย่างชัดเจน
