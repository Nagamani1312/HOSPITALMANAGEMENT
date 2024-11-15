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


GETTING INTO THE PROJECT:
Hospital Management System in Fiori. This system has a ‘Home’ page from where the patient, doctor & administrator can login into their accounts by toggling the tabs accordingly. Fig 1.1 shows the ‘Home’ page of our project.

The ‘Home’ page consists of 3 modules:

1.Patient Module
2.Doctor Module
3.Admin Module
Patient Module:
      This module allows patients to create their account, book an appointment to see a doctor and see their appointment history. The registration page(in the home page itself) asks patients to enter their First Name, Last Name, Email ID, Contact Number, Password and radio buttons to select their gender.

Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard(Fig 1.5).

The Dashboard page allows patients to perform two operations:

1. Book his/her appointment:

      Here, the patients can able to book their appointments to see a doctor. The appointment form(Fig 1.6) requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.


After clicking on the ‘Create new entry’ button, the patient will receive an alert that acknowledges the successful appointment of the patient.(See Fig 1.7)

2. View patients’ Appointment History:

      Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.(See Fig 1.8).

 Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again. Fig 1.9 shows the login page. Clicking on ‘Login’ button will redirect the patient to his dashboard page which we have seen earlier (Fig 1.5)

image

This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history.

Doctor Module:
      The doctors can login into their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’. Fig 1.10 shows the login form for a doctor. Registration of a doctor account can be done only by admin. We will discuss more about this in Admin Module.

image

Once the doctor clicking the ‘Login’ button, they will be redirected to their own dashboard which is shown in Fig 1.11

image

In this page, doctor can able to see their appointments which has been booked by the patients. Fig 1.12 shows the appointment of the doctor ‘Ganesh’ which has been booked by the patient ‘Kenny Sebastian’ (Fig 1.6). This means that the doctor ‘Ganesh’ will have an appointment with the patient ‘Kenny Sebastian’ on 10-10-2019 10AM.

image

In real-time, the doctors will have thousands of appointments. It will be easier for a doctor to search for appointment in the case of more appointments. To make it easier, I have a ‘Search’ box in the navigation bar (See Fig 1.12) which allows doctors to search for a patient by their contact number.       Once everything is done, the doctor can logout of their account. Thus, in general, a doctor can login into his/her account, view their appointments and search for a patient. This is all about Doctor Module.

Admin Module:
      This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments and the feedback/queries received from the ‘Contact’ page. Also admin can add doctor too.       Login into admin account can be done by toggling into admin tab of the Home page. Fig 1.13 shows the login page for admin.       username: admin, password: admin123

image

On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard as shown in Fig 1.14.

image

This module allows admin to perform five major operations:

1. View the list of all patients registered:

      Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password. (See Fig 1.15).As like in doctor module, admin can also search for a patient by their contact number in the search box.

image

2. View the list of all doctors registered:

      Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees, shown in Fig 1.16. Searching for a doctor can be done by using the doctor’s Email ID in the search box.

image

3. View the Appointment lists:

      Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. (See Fig 1.17).

image

4. Add Doctor:

      Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.(See Fig 1.18)

image

After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the list as shown in the Fig 1.19

image

5. View User’s feedback/Queries:

      Admin is allowed to view the feedback/Query that has been given by the user in the ‘Contact’ page (Refer Fig 1.3). This includes User’s Name, Email Id, Contact Number and the message(Feedback/ Query) as shown in the Fig 1.20.

image

. Cancel Appointments
      Patients and doctors can able to delete their appointments.

image

If the patient deletes the last record (for doctor Ganesh), then a label "deleted by you" will be displayed in the column 'Current Status' and the action will change to cancel state.

image

Now if we login to the doctor Ganesh's account and view his appointment details, then it will look like this:

image

Similarly doctors can also delete their appointments and patients can view their updated appointment details.

2. Remove Doctors by Admin
      Admin can also delete the doctors from the system. This let admin to have more control over the system.

image
      Taking everything into consideration, admin can able to view the details of patients and doctors, appointment details, Feedback by the user and can add a new doctor. Once everything is done, the admin can logout from his account.
