# Medicare
Medicare is a medical app for android platform which will keep information about patients visiting the hospital. 
App will be used by patient’s visiting the hospital, Secretaries and doctor’s. 
The main purpose of the app is to keep a record of patients where the secretary can open a file of patients, a doctor can add necessary details, keep a record of medical expenses , patient can view all the information related to him/her, do emergency chat with doctor when required.
There will be mainly 3 users using the app. Doctor, Secretary and Patient. Doctors and secretary have to register in order to use the app
In a scenario where a patient went to a hospital to have a meeting with a doctor.


Secretary: A secretary job is to deal with patient before he/she sees the doctor
1.	Secretary will add a new patient to the system. Every patient will be saved under a unique 5 digit file number which will be used further on every step. The secretary has to fill a personal information form for the patient which will include all the information about the patient like name, address, blood group, reason for visit etc.
2.	In case of change of address or phone number which is very common in a day to day scenario, the secretary can edit the information for the patient. (Nurse can edit info like address, phone number, emergency contact name but cant change infos like patient name, age or blood group)
3.	Secretary has to put the medical expenses for the patient. She will add costs related to consultation, reports, pharmacy etc.
4.	Secretary has to clear bills so she can enter the amount paid by the patient and update it in the patient file. This way she can keep a record of what are medical expenses for each patient and how much amount is paid and also the mode of payment.
5.	The secretary can see the whole list of patients ever registered in the system (secretary can see personal info but not the medical history or medicines).
6.	Secretary can see the list of doctors registered in the system with their name, phone number and email.


Doctor: A doctor's job is to see the patient. Before seeing the doctor, patient is already registered in system and he/she have a file number which have all of his/her info
1.	Doctors can add medical reports related info and create a medical history for the patient. In case if a medical report is already there, the old report will be shown in fields and the doctor can edit it or can add more stuff to it. The logic behind this is to give advantage to doctors. In a day to day scenario where doctors are usually specialized in something particular to the human body, patients usually have to see more than 1 doctor in a hospital. In such cases, if the report has already been uploaded by a doctor, if the patient sees another doctor and the doctor wants to make a report, he/she can see the old report which he can edit or add new things in the existing one.
2.	Doctors can add medicines  with dosage and days to the file of patients. Each input will be followed by starting date and end date. In this scenario old medicines will also remain there and every time, a new medicine will be added with starting day till the day it has to be continued.
3.	Doctors can see the patient info, medical expenses, add, update the medical expenses, do the billing, see in depth of the patient profile with his personal info, billing info, medicines, medical reports etc etc.
4.	Doctors can see the list of patients registered and can view medical history of any patient which a secretary can’t see.
5.	Doctor can see the list of secretaries registered in system
6.	Doctors will have an option of emergency chat with patients. In this chat, he/she can send a text or reply to a patient. It iss like a messaging feature inside the app


Patient: A patient wants to keep a record of his medical history and medicines and can view them when needed.
1.	Patients can enter the file number and see all the info related to him/her.
2.	Patient doesn’t need to login or register to the system. He/she can just enter the file number and view all the personal info, medical history and medicines consulted by the doctor and his billing details.
3.	Patients can message the doctor in case of emergency. There is a full fledged messaging feature where patients can send a message to the doctor in case of emergency.
4.	Whenever a patient will open his file using file number, in case if he had received a message from a doctor, he will be notified and get a toast message as well.

Information about the Doctor login:

Id: Manish@gmail.com
Password 123456
Id. Harish@gmail.com
Password. 123456
Id. Mohammad@gmail.com
Password. 123456

Information about the Secretary login:
Id: Dinkar123@gmail.com
Password: 123456


Some patients File numbers
13248
55553
51849 

You can register in system for both doctor and secartey.Once registered you can made a new file number using add
Note: new patient in secretary dashboard


Hospital is the end users for this Application because it needs this app for their system to work smooth and easy. 
Thus, hospital can keep a record of patients visitng the hospital and secretry, doctor can use this application for their convenience.

 Medicare gives the ability to optimize and digitize all the processes within the institution, which will help to improve customer service, reduce process costs, streamline the search of medical records, bills, patients, doctors, etc. 
 thus, having a database of each module implemented needs application for the easy and usefull system.
 
 Technology used
 

Android Studio (version 3.5.5)
Java
Firebase Realtime Database
Firebase Authentication


Medciare tries to digitize all the processes within the institution thus it need to have many features which are needed to fulfil the demands of end user. Kepping app optimised and feature loaded was  agreate challange. We had to take in account that app dont crashes at any point.
We built a emergency chat system within the system. Making a chat system is always a tough job. We tried using our full potential to use the real time database for making a simple yet effective chat.
One big problem with chat was we have to save each message in the same order as sent and we have to show it in same order too.

One more task in chat system was to show a notification in any form to the user and doctor so that he/she gets to know about a message. We tried a different approach and tried our level best to make it presentable and useful
Doctors, secretary have to login in order to use the app. Patients mainly have to enter his/her file number to see his info. In cases where medical reports or medicines are not inputted by a doctor, it will show as info is not inputted yet.
We are using firebase authentication for the login. Secretary Doctors can register with some basic info and can also reset passwords in case of forgetting the password. Patients don't have to register using email passwords. They can access their file using a 5 digit file number.
All the data will be processed and saved from the realtime database. All the passwords are saved using firebase authentication.
A limitation we see in app is reinputting the file number again and again on doctor side. We can resolve it if taken into consideration at beigining of the project but due to lack of time we have to keep it as it is.
The problem with this limitation is when a patient arries to doctor, doctor usually have to enter reports, medicines and other things all at same time but he have to renter file number at every sustem. We can simply set a variable which can carry file number to every feature until doctor doesn’t reset it.
