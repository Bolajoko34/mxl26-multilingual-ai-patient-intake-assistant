# MxL26 | Multilingual AI Patient Intake Assistant
Status: Prototype | English version complete | Local language integration in progress

## Overview
MxL26 is an AI-powered patient intake assistant built for Ghanaian healthcare facilities. It collects patient information before they see a healthcare worker, reducing language barriers, crowding, and waiting time at the point of care.
MxL26 is not a diagnostic tool. It does not prescribe medicine, recommend treatment, or make clinical decisions. Its sole purpose is to collect and organize patient intake information for healthcare staff.

## The Problem It Solves
Many patients in Ghanaian healthcare facilities speak little or no English. This creates delays, miscommunication, and longer wait times. Frontline staff spend time collecting basic intake information that a tool like MxL26 handles automatically, freeing them to focus on care.

## What MxL26 Does
* Greets patients and asks for their preferred language before starting.
* Collects intake information in this order: hospital card status, patient type, health insurance, reason for visit, age, location, occupation, marital status, symptoms, medicines taken, allergies, and urgent warning signs.
* Detects emergencies. If a patient mentions difficulty breathing, chest pain, severe bleeding, fainting, or seizures, MxL26 stops the intake and directs staff to attend to the patient immediately.
* Flags unaccompanied minors and alerts staff before continuing.
* Handles patients who stop responding by prompting once, then alerting staff.
* Redirects medical questions. If a patient asks for a diagnosis or prescription, MxL26 acknowledges them and redirects to a healthcare worker.
* Generates a structured intake summary at the end of every session for healthcare staff to review.

## Sample Intake Summary Output
Emergency case: No
Patient name: Abena Mensah
Languages used: English
Hospital card opened today: Yes
Patient status: Returning patient
Health insurance: Yes
Health insurance status: Active
Age: 34
Unaccompanied minor: N/A
Location: Kumasi, Ashanti Region
Occupation: Trader
Marital status: Married
Reason for visit: Follow-up
Visit type: Returning
Service needed: Prescription refill
Last hospital visit: Two weeks ago
Reason for return: Collect medication
Documents available: Prescription
Symptoms: Mild headache
Duration of symptoms: 3 days
Medicine taken: Paracetamol
Allergies: None
Urgent warning signs: None
Suggested next step: Standard intake complete. Patient ready to see healthcare worker.

## Language Support
English: Tested and functional.
In development: Twi, Ga, Hausa, Ewe, Fante, Dagbani, Dangme, Mooré, and natural mixtures of these languages.
MxL26 is designed to follow patients who switch languages mid-conversation, and to handle Ghanaian accents, local medicine names, and transcription errors from speech-to-text input.

## Tools and Technologies
Generative AI, Prompt Engineering, Vapi

Project Structure
README.md | Project documentation
system_prompt.md | Full MxL26 system prompt
sample_output.md | Example intake summary

Current Limitations
Local language support is still in active iteration. MxL26 defaults to simple English when it is not confident enough in a language to phrase a medical question correctly.
This is a prototype. It has not been deployed in a clinical setting.

What Is Next
Complete local language integration across all 11 supported languages.
Test with real patients in a Ghanaian healthcare facility.
Explore integration with hospital management systems.

