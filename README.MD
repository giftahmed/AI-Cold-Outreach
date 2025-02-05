Here’s a properly structured README file for your project:

---

# AI-Powered Cold Outreach System

This project automates the cold outreach process for the German market, specifically targeting leads in the real estate sector. The system scrapes leads from ImmobilienScout24, personalizes outreach emails, and automates email delivery using Microsoft Power Automate.

## Tools Used

1. **Instant Data Scraper**: A web scraping tool to extract lead data from ImmobilienScout24.
2. **Microsoft Excel**: Used to store and organize the scraped lead data.
3. **Microsoft OneDrive**: Stores the Excel file for easy access and updates.
4. **Microsoft Power Automate**: Automates the email personalization and delivery process.

## Process Overview

### 1. Lead Scraping:
- **Website**: [ImmobilienScout24](https://www.immobilienscout24.de/Suche/de/baden-wuerttemberg/neubauwohnungen)
- **Tool**: Instant Data Scraper
- **Columns Scraped**:
  - Website
  - Project Name
  - Location
  - Contact Person
  - Company Name
  - Email
- **Output**: The scraped data is saved in an Excel file (`Leads.xlsx`).

### 2. Data Organization:
- The Excel file was reviewed to ensure all columns were populated correctly.
- The file was uploaded to Microsoft OneDrive for seamless integration with Power Automate.

### 3. Email Automation:
- **Tool**: Microsoft Power Automate
- **Steps**:
  1. Created a flow to read data from the OneDrive Excel file.
  2. Scheduled the flow to run automatically on Mondays and Wednesdays.
  3. Personalizes the email content dynamically using columns from the Excel file.
  4. Sent a test email to ensure the flow works correctly.

#### Email Template:

```
Subject: Maximale Sichtbarkeit für Ihr Projekt {Project Name} in {Location}

Sehr geehrte/r {Contact Person},

Ich hoffe, diese Nachricht erreicht Sie wohlbehalten. Mein Name ist [Ihr Name], und ich bin von ExposeProfi. Wir unterstützen Immobilienentwickler wie {Company Name} dabei, ihre Projekte durch professionelle Fotografie, virtuelle Touren und KI-gestützte Marketinglösungen erfolgreich zu vermarkten.

Ich habe gesehen, dass Sie derzeit das Projekt {Project Name} in {Location} entwickeln. Unsere Dienstleistungen könnten Ihnen helfen, die Sichtbarkeit Ihres Projekts zu maximieren und potenzielle Käufer oder Mieter effektiv anzusprechen.

Wären Sie an einem kurzen Gespräch interessiert, um mehr über unsere Lösungen zu erfahren? Ich würde mich freuen, Ihnen zu zeigen, wie wir Sie bei der Vermarktung Ihres Projekts unterstützen können.

Mit freundlichen Grüßen,  
Ihr Name  
Position  
ExposeProfi  
Kontaktdaten
```

### 4. Testing and Validation:
- Tested the flow to ensure it reads the Excel file correctly, personalizes the emails, and sends them to the intended recipients.
- Verified that the flow runs on the scheduled days (Mondays and Wednesdays).

### 5. Exporting the Solution:
- Exported the Power Automate flow as a solution package.
- Attached the solution package for easy replication.

## Steps to Replicate the Flow

### 1. Download the Solution Package:
- Locate and download the attached solution package in this folder.
- Import the solution into your Microsoft Power Automate account.

### 2. Set Up the Excel File:
- Upload the provided `Leads.xlsx` file to your OneDrive.
- Ensure the file contains the following columns:
  - Website
  - Project Name
  - Location
  - Contact Person
  - Company Name
  - Email

### 3. Configure the Flow:
- Open the imported flow in Power Automate.
- Update the connection to point to your OneDrive Excel file.
- Review and customize the email template if needed.

### 4. Test the Flow:
- Run the flow manually to ensure it works as expected.
- Verify that the emails are personalized and sent correctly.

### 5. Schedule the Flow:
- Set the flow to run automatically on your preferred schedule (e.g., Mondays and Wednesdays).

## Folder Structure:
- **Leads.xlsx**: Contains the scraped lead data.
- **AIColdOutreach.zip**: Exported Power Automate flow for replication.
- **Documentation.docx**: This documentation file.
- **Email_Template.txt**: The Email Template

## Limitations and Future Improvements

### Limitations:
- The current system is limited to 20 leads due to the scope of the task.
- Free tiers of Power Automate may have usage limits.

### Future Improvements:
- Scale the system to handle larger datasets by upgrading to a paid Power Automate plan.
- Integrate additional data sources (e.g., LinkedIn, local business directories) for richer lead information.

### **Demo Video**
Watch a walkthrough of the app's features and codebase:  
**[Demo Video Link](hhttps://youtu.be/lnZjE8chtHU)**