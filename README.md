## Application Details
|               |
| ------------- |
|**Generation Date and Time**<br>Tue Sep 10 2024 09:31:21 GMT+0000 (Coordinated Universal Time)|
|**App Generator**<br>@sap/generator-fiori-freestyle|
|**App Generator Version**<br>1.14.5|
|**Generation Platform**<br>SAP Business Application Studio|
|**Template Used**<br>simple|
|**Service Type**<br>SAP System (ABAP On Premise)|
|**Service URL**<br>http://sapbtp.com:8023/sap/opu/odata/sap/ZHM_PROJECT_SRV|
|**Module Name**<br>hospitalmanage|
|**Application Title**<br>Hospital Management|
|**Namespace**<br>|
|**UI5 Theme**<br>sap_horizon|
|**UI5 Version**<br>1.114.0|
|**Enable Code Assist Libraries**<br>False|
|**Enable TypeScript**<br>False|
|**Add Eslint configuration**<br>False|

## hospitalmanage

An SAP Fiori application.

### Starting the generated app

-   This app has been generated using the SAP Fiori tools - App Generator, as part of the SAP Fiori tools suite.  In order to launch the generated app, simply run the following from the generated app root folder:

```
    npm start
```

- It is also possible to run the application using mock data that reflects the OData Service URL supplied during application generation.  In order to run the application with Mock Data, run the following from the generated app root folder:

```
    npm run start-mock
```

#### Pre-requisites:

1. Active NodeJS LTS (Long Term Support) version and associated supported NPM version.  (See https://nodejs.org)


#### GETTING INTO THE PROJECT:

Hospital Management System in Fiori. This system has a ‘Home’ page from where the patient, doctor & administrator can login into their accounts by toggling the tabs accordingly. 
The ‘Home’ page consists of 3 modules:
1.Patient Module
2.Doctor Module
3.Admin Module
![image](https://github.com/user-attachments/assets/7e16b95d-5611-4feb-bdd1-86476c6d710a)


##Patient Module:
      This module allows patients to create their account, book an appointment to see a doctor and see their appointment history. The registration page(in the home page itself) asks patients to enter their First Name, Last Name, Email ID, Contact Number, Password and radio buttons to select their gender.

Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard.
![patient module](https://github.com/user-attachments/assets/7d9074fb-872e-4a81-b552-4acf56064b93)


The Dashboard page allows patients to perform two operations:

1. Book his/her appointment:

      Here, the patients can able to book their appointments to see a doctor. The appointment form(Fig 1.6) requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.
![bookappointment](https://github.com/user-attachments/assets/be9277f5-78b6-4d7f-9fc3-25892e64b3fb)




2. View patients’ Appointment History:

      Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.
   ![booking,cancelling](https://github.com/user-attachments/assets/aad4bb1e-b3aa-4a93-acee-af10c651eba4)


 Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again.
2. View patients’ prescriptions:

      Here, the patient can see their prescriptions history which are given by particular doctor.

 Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again.

This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history and prescriptions given by doctor.

## Doctor Module:
      The doctors can login into their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’. The figure shows the login form for a doctor. Registration of a doctor account can be done only by admin. We will discuss more about this in Admin Module.
![doctor login](https://github.com/user-attachments/assets/0e6d316a-f78f-40b0-96ff-4dbc5f1b8d1c)




Once the doctor clicking the ‘Login’ button, they will be redirected to their own dashboard which is shown in below figure.

![doctor page](https://github.com/user-attachments/assets/b8ab66d7-27ee-4db9-b974-85ef19e6e935)

In this page, doctor can able to see their appointments which has been booked by the patients. The below Figure shows the appointment of the doctor ‘Ganesh’ which has been booked by the patient. This means that the doctor ‘Ganesh’ will have an appointment with the patient on 10-10-2019 10AM.

![appointments](https://github.com/user-attachments/assets/7475a7b2-0a6b-4686-bc4e-4652bdfc5a54)


In this page, doctor can able to give prescriptions to the patients .  shows the appointment of the doctor ‘Ganesh’ which has been booked by the patient ‘Ram’. This means that the doctor ‘Ganesh’ will have an appointment with the patient ‘Ram’ on some particular date and he can can either cancel the appointment or can accept the appaointment.
![prescriptiongiven](https://github.com/user-attachments/assets/8451042d-6609-46ed-bada-77dda9ccc4fd)

## Admin Module:
      This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments. Also admin can add doctor too.Login into admin account can be done by toggling into admin tab of the Home page. 
![image](https://github.com/user-attachments/assets/559516bc-37b3-4389-892e-9068ed247ecd)


On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard as shown in Figure.
![admin home](https://github.com/user-attachments/assets/12d70e62-fefc-410f-85a1-d20bfbbd1f0b)




This module allows admin to perform five major operations:

1. View the list of all patients registered:

      Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password.
![patient list](https://github.com/user-attachments/assets/cc7adc4c-43e3-40bb-bda0-a23f0adaacf3)



2. View the list of all doctors registered:

      Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees, shown in Fig 1.16. Searching for a doctor can be done by using the doctor’s Email ID in the search box.
![doctor list](https://github.com/user-attachments/assets/c66da06c-67a1-4b70-b6e7-0fe36cb24299)



3. View the Appointment lists:

      Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. (See Fig 1.17).
![appointment details](https://github.com/user-attachments/assets/5ae2431c-f866-46f1-8537-46df40f3a84e)



4. Add Doctor:

      Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.
![adddoctor](https://github.com/user-attachments/assets/3656d12f-59ce-4586-a8b8-243967dd15fd)



After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the Doctors list 
. Cancel Appointments
      Patients and doctors can able to delete their appointments.
If the patient deletes the last record (for doctor Ganesh), then a label "deleted by you" will be displayed in the column 'Current Status' and the action will change to cancel state.
![booking,cancelling](https://github.com/user-attachments/assets/3f36f418-948f-44ba-ab41-a33b0cada198)



Now if we login to the doctor Ganesh's account and view his appointment details.The doctors can also delete their appointments and patients can view their updated appointment details.
![appointments](https://github.com/user-attachments/assets/14ba3c11-0d75-4235-ad83-37c69e0a2a3f)

5. Remove Doctors by Admin
      Admin can also delete the doctors from the system. This let admin to have more control over the system.
![delete doctor](https://github.com/user-attachments/assets/26841d24-5900-4835-9ac9-4496f5c7b44f)

      Taking everything into consideration, admin can able to view the details of patients and doctors, appointment details,delete a doctor and can add a new doctor. Once everything is done, the admin can logout from his account.
