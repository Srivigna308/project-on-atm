# project-on-atm
3 verifications for an atm that is cardless like face recognition, family access, otp 

💡 Project Title:
Facial Recognition Based ATM System with Multi-Layered Verification Options

📘 Project Overview:

This project presents a secure, cardless ATM system that enhances security and user experience through facial recognition, family access authorization, and OTP-based verification. Instead of relying on physical ATM cards, users authenticate using an account number and password, followed by one of three advanced verification methods, before accessing typical ATM services such as transfer, balance inquiry, deposit, and withdrawal.

 🔐 Authentication & Verification Flow:

 1. Initial Login:

* User inputs:

  * Account Number
  * Password
* If credentials match the stored data, proceed to verification phase.

2. Secondary Verification Options (User Chooses One):

✅ Option 1: Facial Recognition

* The system uses a camera to scan the user’s face.
* Facial data is compared against the **registered facial biometric** stored in the bank database.
* If match is confirmed, user is authenticated.

Tools/Technologies:

* OpenCV /  Deep Learning (FaceNet, dlib, etc.)



 ✅ Option 2: Family Access (Alternate User Verification)

* For users unable to access their account (e.g., elderly), a **pre-authorized family member** can verify on their behalf.
* Family member inputs:

  * Their registered **mobile number/email**
  * **Password or PIN**
* The system confirms their identity from a linked family access list.

Use Case Example:
An elderly parent can't remember their password, so their child can authorize on their behalf using linked credentials.



✅ Option 3: OTP Verification

* An **OTP (One Time Password)** is sent to the user’s **registered mobile number or email**.
* User enters the OTP within a given time window.
* If the OTP is valid, verification is successful.


 📋 Post-Verification: Functional Dashboard

Once any one of the verification methods is successful, the user is granted access to the main ATM functionalities.

 Main Dashboard Options:

1. 🔁 Money Transfer

   * Send money to another account.
   * Input: Receiver's account number, amount, optional message.

2. 📊 Balance Enquiry

   * Displays current account balance.
   * May include mini-statement or recent transactions.

3. 💰 Deposit

   * Simulates cash or cheque deposit.
   * Input: Amount to deposit.
   * Balance is updated accordingly.

4. 🏧 Withdraw

   * Withdraw funds from the account.
   * Input: Amount to withdraw.
   * Ensures sufficient balance is available.

5. 🚪 Logout

   * Ends session and redirects to the login page.


 🔄 System Workflow Summary:


Start

  ↓
  
Enter Account Number & Password

  ↓
  
If valid → Show 3 verification options:

  → 1. Facial Recognition
  
  → 2. Family Access
  
  → 3. OTP
  
  ↓
  
If any verification is successful

  ↓
  
Access Main Dashboard

  ↓
  
Choose Function (Transfer / Balance / Deposit / Withdraw)

  ↓
  
After operation, choose to Logout or return to Dashboard

  ↓
  
End


