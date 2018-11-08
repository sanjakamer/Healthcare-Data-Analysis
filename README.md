# Health Insurance Claims Analysis with Pandas
Author: **Amer Sanjak**<br>
email:sanjakam@gmail.com

In this tutorial, we will examine claims data set that was extracted from an Electronic Medical Records Billing System that I designed, developed and implemented in the United States.  

Medical billing is a payment practice within the United States health system. The process involves a healthcare provider submitting, and following up on, claims with health insurance companies in order to receive payment for services rendered; such as treatments and investigations.

The DataFrame we will be examining contains the following columns:

claimid
billedamount


status
dos
provider
insurance
patientid
dob
sex
city
state
zipcode


1. **claimid:** This is the primary key for the claims DataFrame
1. **billedamount:** The amount billed by the provider to the insurance company for provided  to patient
1. **paidamount:** The amount paid by insurance company to provider for the claim
1. **status:** Claim status category
1. **dos:** Data of service
1. **paiddate:** Paid date by insurance company
1. **provider:** Provider name -  real provider name has been removed
1. **insurance:** Insurance company name
1. **patientid:** Patient medical record number 
1. **dob:** Patient's date of birth
1. **sex:** Patient gender


# Table of Content
### 1. Basic Setup

<ul>
   <li><a href="#A1">1.1 Version Information</a></li>
   <li><a href="#A2">1.2 Import all Packages</a></li>
   <li><a href="#A3">1.3 Style Function</a></li>
   <li><a href="#A4">1.4 Import CSVs files</a></li>
   <li><a href="#A5">1.5 Print First Five Records</a></li>
</ul>

### 2. Data Cleaning
<ul>
  <li><a href="#B1">2.1 Missing Values</a></li>
  <li><a href="#B2">2.2 Examin Missing Values</a></li>
  <li><a href="#B3">2.3 Drop Empty Rows</a></li>
  <li><a href="#B4">2.4 Convert date string columns with the .to_datetime() method</a></li>
  <li><a href="#B5">2.5 Create New Fields</a></li>  
</ul>

### 3. Data Analysis
<ul>
  <li><a href="#C1">3.1 Visit Statistics</a></li>
    <ul>
        <li><a href="#C311">3.1.1 Visits count Using unstack() method</a></li>
        <li><a href="#C312">3.1.2 Visits count Using crosstab() method</a></li>
        <li><a href="#C313">3.1.3 Visits count Using Group method</a></li>
        <li><a href="#C314">3.1.4 Plot Visit Count by Month</a></li>
        <li><a href="#C315">3.1.5 Age Group</a></li>
        <li><a href="#C316">3.1.6 Patient Visits by Gender</a></li>
        <li><a href="#C317">3.1.7 Patients by City</a></li>
        <li><a href="#C318">3.1.8 Patients by Zipcode</a></li>
    </ul>
</ul>
<ul>
  <li><a href="#D1">4.1 Revenues and Insurance  Statistics</a></li>
    <ul>
        <li><a href="#D411">4.1.1 Revenues by Month </a></li>
        <li><a href="#D411">4.1.2 Descriptive Statistics</a></li>
        <li><a href="#D412">4.1.3 Claims by Status Category </a></li>
        <li><a href="#D413">4.1.4 Patient Assignments by Insurance</a></li>
    </ul>
</ul>
