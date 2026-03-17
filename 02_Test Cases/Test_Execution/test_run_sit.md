# Nomi Test Cases

---

## Scenario: User Login Verification

---

### TC_001 — Validating Valid Username and Password login

**Execution Details:**
Execution Date: 16-Mar-2026
Executed By: Dinesh Subramaniyan
Build Version: 
Status: Pass
Remarks: Working as expected

**Preconditions:**
- Application URL is accessible
- Valid Username and Password
- User has Entra access

**Steps:**

1. Navigate to the Application URL.
2. Enter valid username and password and click on the Sign In button.
3. Capture screenshot after user landed on home screen.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. User is navigated to ENTRA SSO for authentication. After successful authentication, user lands on the Takeda "One Evidence Synthesis Platform" Home Page.

**Actual Results:**

1. User was successfully redirected to the Takeda login page.
2. ENTRA SSO authentication was completed successfully.
3. User landed on the Takeda **"One Evidence Synthesis Platform" Home Page**.
4. Screenshot captured after landing on the home screen.

---

### TC_002 — Validate Login with Valid Username and Empty Password

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- Valid username is available
- User has Entra access

**Steps:**

1. Navigate to the Application URL.
2. Enter a valid username and leave the **Password** field empty.
3. Click on the **Sign In** button.
4. Capture a screenshot with the error message.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays the message **"Please enter your password."**

**Actual Results:**

1. User was redirected to the Takeda login page.
2. System displayed the validation message **"Please enter your password."**

---

### TC_003 — Validate Login with Valid Username and Invalid Password

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- Valid username and invalid password are available
- User has Entra access

**Steps:**

1. Navigate to the Application URL.
2. Enter a valid username and an invalid password.
3. Click on the **Sign In** button.
4. Capture a screenshot with the error message.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays the message:  
   **"Your account or password is incorrect. If you don't remember your password, reset it now."**
3. User is not logged in and remains on the login page.

**Actual Results:**

1. User was redirected to the Takeda login page.
2. System displayed the message:  
   **"Your account or password is incorrect. If you don't remember your password, reset it now."**
3. User remained on the login page and was not logged in.

---

### TC_004 — Validate User Accessing the NOMI Application from a Non-Takeda Environment

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version: V1.0  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- User is accessing the application from a non-Takeda environment

**Steps:**

1. Navigate to the Application URL.

**Expected Results:**

1. User receives a **"Site can't be reached"** error message.
2. User is unable to access the NOMI application.

**Actual Results:**

1. When accessing the application URL from a non-Takeda environment, the browser displayed the **"Site can't be reached"** error message.
2. User was unable to access the NOMI application.
---


### TC_005 — Validate Login Attempt Without Entering Username

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible

**Steps:**

1. Navigate to the Application URL.
2. Leave the **Email** field empty and click the **Next** button.
3. Capture a screenshot with the error message.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays the message:  
   **"Enter a valid email address, phone number, or Skype name."**
3. User is not logged in and remains on the login page.

**Actual Results:**

1. User was redirected to the Takeda login page.
2. When the **Next** button was clicked without entering a username, the system displayed the message:  
   **"Enter a valid email address, phone number, or Skype name."**
3. User remained on the login page.
---

### TC_006 — Validate Error Message for Invalid Email Domain

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- Invalid email address

**Steps:**

1. Navigate to the Application URL.
2. Enter an email address with an invalid domain name.
3. Click **Next**.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays the message **"We couldn't find an account with that username."**
3. User is not logged in and remains on the login page.

**Actual Results:**

1. User was redirected to the Takeda login page.
2. After entering an email with an invalid domain, the system displayed the message **"We couldn't find an account with that username."**
3. User remained on the login page and was not logged in.

---

### TC_007 — Validate Error Message for Invalid Username with Correct Domain

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- Invalid username with correct domain

**Steps:**

1. Navigate to the Application URL.
2. Enter an invalid username with the correct domain email address.
3. Click **Next**.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays the message **"The username may be incorrect. Make sure you typed it correctly or contact your admin."**
3. User is not logged in and remains on the login page.

**Actual Results:**

1. User was redirected to the Takeda login page.
2. System displayed the message **"The username may be incorrect. Make sure you typed it correctly or contact your admin."**
3. User remained on the login page and was not logged in.

---

## Scenario: Validating the Home Page

---

### TC_008 — Validate the Home Page

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version: V1.0  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- Valid username and password
- User has Entra access

**Steps:**

1. Log in to the application and navigate to the **Home Page**.
2. Verify that **Upload File**, **Recent Files**, and **LuminiAI Portal** options are displayed.
3. Verify that the **user email and Logout icon** are displayed in the top-right corner.
4. Click the **Logout** icon.

**Expected Results:**

1. After successful login, **Upload File**, **Recent Files**, and **LuminiAI Portal** options are visible on the Home Page.
2. User email and **Logout** icon are displayed in the top-right corner.
3. User is successfully logged out of the application.

**Actual Results:**

1. After login, **Upload File**, **Recent Files**, and **LuminiAI Portal** options were visible on the Home Page.
2. User email and **Logout** icon were displayed in the top-right corner.
3. User clicked the **Logout** icon and was successfully logged out of the application.

---

## Scenario: File Upload Through Select PDF File

---

### TC_009 — Validate Valid PDF Upload Through File Browser

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Error observed — bug raised  

**Preconditions:**
- User is successfully logged in
- Valid PDF file available

**Steps:**

1. On the Takeda Home Page, under the **Upload File** section, click **Start Processing**.
2. Verify that **Home**, **Upload File**, **Recent Files**, and **LuminiAI Portal** options are displayed in the top-right corner along with the **user email and Logout button**.
3. Select **Therapeutic Area = GI** and **Document Type = Manuscript**, then click **Select PDF File**.
4. In the File Explorer window, choose a PDF file and click **Open**.

**Expected Results:**

1. System navigates to the upload page without errors.
2. Navigation options, user email, and Logout button are visible in the top-right corner.
3. File Explorer opens and allows only **PDF files** to be selected.
4. Selected file name and file size are displayed in the **Upload File** section.
5. File status shows **"Ready to Process"**.
6. **Begin Synthesization** and **Replace Article** buttons are enabled.

**Actual Results:**

1. System navigated to the upload page successfully.
2. Navigation options, user email, and Logout button were visible in the top-right corner.
3. File Explorer opened and allowed selection of PDF files only.
4. Selected file name and file size were displayed in the **Upload File** section.
5. File status was displayed as **"Ready to Process"**.
6. **Begin Synthesization** and **Replace Article** buttons were enabled.

---

### TC_010 — Validate Invalid File Upload Through File Browser

**Execution Details:**  
Execution Date: 05-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- User is successfully logged in
- Invalid file format available

**Steps:**

1. On the Takeda Home Page, under the **Upload File** section, click **Start Processing**.
2. Select **Therapeutic Area = GI** and **Document Type = Manuscript**.
3. Click the **Select PDF File** button.

**Expected Results:**

1. User is navigated to the **Upload File page**.
2. File Explorer opens and allows selection of **only PDF files**.
3. Files with other formats are not selectable.

**Actual Results:**

1. User was navigated to the **Upload File page**.
2. File Explorer opened successfully.
3. Only **PDF files were selectable**, and other file formats were not allowed.
4. Application behaved as expected.

---

## Scenario: Drag and Drop File Upload

### TC_011 — Validate Valid File Drag-and-Drop Upload

**Execution Details:**  
Execution Date: 05-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- User is successfully logged in
- Valid PDF file is available

**Steps:**

1. On the Takeda Home Page under the **Upload File** section, click **Start Processing**.
2. Select **Therapeutic Area = GI** and **Document Type = Manuscript**.
3. Drag and drop a valid PDF file into the upload area.
4. Capture a screenshot of the page.

**Expected Results:**

1. User is navigated to the **Upload File page**.
2. Selected file name and file size are displayed.
3. File status is **"Ready to Process"**.
4. **Begin Synthesization** and **Replace Article** buttons are enabled.

**Actual Results:**

1. User was navigated to the **Upload File page**.
2. After dragging and dropping the valid PDF file, the file name and size were displayed.
3. File status changed to **"Ready to Process"**.
4. **Begin Synthesization** and **Replace Article** buttons were enabled.

---

### TC_012 — Validate Invalid PDF File Through Drag-and-Drop

**Execution Details:**  
Execution Date: 05-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- User is successfully logged in
- Invalid or corrupted PDF file available

**Steps:**

1. On the Takeda Home Page under the **Upload File** section, click **Start Processing**.
2. Select **Therapeutic Area = GI** and **Document Type = Manuscript**.
3. Drag and drop the invalid PDF file.
4. Click **Begin Synthesization**.

**Expected Results:**

1. User is navigated to the **Upload File page**.
2. File name and file size are displayed.
3. When processing starts, the system throws an **error message** indicating the file is invalid.

**Actual Results:**

1. User was navigated to the **Upload File page**.
2. File was uploaded but when **Begin Synthesization** was clicked, the system detected the invalid file.
3. An **error message was displayed**, preventing the processing.

---

### TC_013 — Validate Invalid File (XLSX) Format Through Drag-and-Drop

**Execution Details:**  
Execution Date: 05-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- User is successfully logged in
- XLSX file available

**Steps:**

1. On the Takeda Home Page under the **Upload File** section, click **Start Processing**.
2. Select **Therapeutic Area = GI** and **Document Type = Manuscript**.
3. Drag and drop an **XLSX file** into the upload area.

**Expected Results:**

1. User is navigated to the **Upload File page**.
2. The application does **not allow uploading XLSX files**.

**Actual Results:**

1. User was navigated to the **Upload File page**.
2. When an XLSX file was dragged and dropped, the application **did not allow the file to be uploaded**.

---

### TC_014 — Validate Invalid File (DOC) Format Through Drag-and-Drop

**Execution Details:**  
Execution Date: 05-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- User is successfully logged in
- DOC file available

**Steps:**

1. On the Takeda Home Page under the **Upload File** section, click **Start Processing**.
2. Select **Therapeutic Area = GI** and **Document Type = Manuscript**.
3. Drag and drop a **DOC file** into the upload area.

**Expected Results:**

1. User is navigated to the **Upload File page**.
2. The application does **not allow uploading DOC files**.

**Actual Results:**

1. User was navigated to the **Upload File page**.
2. When a DOC file was dragged and dropped, the application **rejected the file format**.

---

### TC_015 — Validate Invalid File (CSV) Format Through Drag-and-Drop

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- User is successfully logged in
- CSV file available

**Steps:**

1. On the Takeda Home Page under the **Upload File** section, click **Start Processing**.
2. Select **Therapeutic Area = GI** and **Document Type = Manuscript**.
3. Drag and drop a **CSV file** into the upload area.
4. Capture a screenshot of the page.

**Expected Results:**

1. User is navigated to the **Upload File page**.
2. The system displays an **error message indicating unsupported file format**.

**Actual Results:**

1. User was navigated to the **Upload File page**.
2. When the CSV file was dragged and dropped, the system displayed an **unsupported file format error message**.
3. File upload was prevented successfully.

---

### TC_016 — Validating Valid PDF Article Upload and Replace Article

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- Valid Username and Password
- User has Entra access

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, click the "Select PDF File" button.
3. Click the Open button.
4. Click the Replace Article button.
5. Capture the screenshot.

**Expected Results:**

1. User navigated to upload file page.
2. File Explorer opens to select PDF. Other file types cannot be selected.
3. Selected file name and file size shown. File in "Ready to Process" state. Begin Synthesization and Replace Article buttons are enabled.
4. User navigated back to the file selection page.

**Actual Results:**

1. User navigated to upload file page successfully.
2. File Explorer opened and allowed only PDF selection.
3. File name and size were displayed with **Ready to Process** status.
4. Clicking **Replace Article** navigated the user back to file selection page successfully.

---

### TC_017 — Validating the Valid PDF Article Begin Synthesization Flow

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL is accessible
- Valid Username and Password
- User has Entra access

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, click the "Select PDF File" button.
3. Click the Open button.
4. Click the "Begin Synthesization" button.
5. Capture the screenshot.
6. Verify the details displayed on the Preview page (Table Check).

**Expected Results:**

1. User navigated to upload file page.
2. File Explorer opens. Other file types cannot be selected.
3. Selected file name and file size shown. File in "Ready to Process" state. Begin Synthesization and Replace Article buttons are enabled.
<!-- 4. Process takes more than 4 seconds. File extraction starts. Verify file is present in S3 path (/PATH). Check values in: T1 - User File Table, T2 - Extraction & Mapping, T3 - Metadata Table, T4 - Template Table, T5 - Curated Output Table. System navigates to Document Processing page (Uploading → Processing pages → Extracting template data → Finalizing). On completion, user is -->navigated to Preview page. 
6. Preview page displays: Run ID, Status, Pipeline Status, Structure Summary, Generated XLSX File Name, Overall Progress (%), Fields Extracted, Quality Score, Template Output Details. Hide PDF and Publish to Lyra buttons are enabled.

**Actual Results:**

1. User navigated to upload file page.
2. PDF file selected successfully.
3. File status displayed as **Ready to Process**.
4. After clicking **Begin Synthesization**, system started processing.
5. System navigated through **Uploading → Processing → Extracting → Finalizing** stages.
6. User was navigated to **Preview Page** with generated results.

---

### TC_018 — Validating Structure Summary for 1st time upload PDF

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page

**Steps:**

1. Navigate to the Structure Summary part and click the extend icon. Validate the details present there.
2. Capture the screenshot.

**Expected Results:**

1. Structure Summary extends showing: Total Pages, Total Headings, Total Tables, Total Figures, Total Text Blocks, Mapped Percentage. Validate counts against the PDF.


**Actual Results:**

1. Structure Summary section expanded successfully.
2. Displayed **Total Pages, Headings, Tables, Figures, Text Blocks and Mapping %**.
3. Values matched the uploaded PDF document.

---

### TC_019 — Validating Structure Summary for same pdf reupload

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page
- Have structure summary data from an existing file upload

**Steps:**

1. Navigate to the Structure Summary part and click the extend icon. Validate the details present there.
2. Validate the structure summary values against previous upload values.
3. Capture the screenshot.

**Expected Results:**

1. Structure Summary extends showing: Total Pages, Total Headings, Total Tables, Total Figures, Total Text Blocks, Mapped Percentage. Validate counts against the PDF.
2. Both sets of values should match.

**Actual Results:**

1. Structure Summary expanded successfully.
2. Values displayed for **pages, headings, tables, figures and text blocks**.
3. Values matched previously uploaded file data.

---

### TC_020 — Study Overview Part

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

*Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page

**Steps:**

1. Navigate to Template Output part and click the Study Overview section extend icon.
2. Capture the screenshot.
3. Click the Add Feedback button.
4. Click the Save button.
5. Click the Edit Feedback button.
6. Click the Show Evidence button.
7. Click the "Open in Preview" button.

**Expected Results:**

1. Overview shows: Study ID, Content Type, Content Status, match accuracy (%) for each part. Each part has Add Feedback and Show Evidence buttons.
3. Feedback section opens with a text box; user can add feedback.
4. Add Feedback button changes to Edit Feedback button.
5. Previously added comments are present in the text box; user can update the existing feedback.
6. Page number is displayed below; Open in Preview button appears.
7. In the right side, the PDF respective page opens and the relevant line is highlighted.

**Actual Results:**

1. Overview section expanded successfully.
2. Study ID, Content Type, Content Status and match accuracy displayed.
3. Feedback was added and saved successfully.
4. **Edit Feedback** button appeared after saving.
5. **Show Evidence** opened PDF preview with highlighted content.

---

### TC_021 — Outcomes and Evidance

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page

**Steps:**

1. Navigate to Template Output part and click the Outcomes and Evidance extend button.
2. Capture the screenshot.
3. Click the Add Feedback button.
4. Click the Save button.
5. Click the Edit Feedback button.
6. Click the Show Evidence button.
7. Click the "Open in Preview" button.

**Expected Results:**

1. Limitations section shows study limitations with match accuracy (%). Add Feedback and Show Evidence buttons are present.
3. Feedback section opens with a text box; user can add feedback.
4. Add Feedback button changes to Edit Feedback button.
5. Previously added comments are present; user can update the existing feedback.
6. Page number is displayed below; Open in Preview button appears.
7. In the right side, the PDF respective page opens and the relevant line is highlighted.

**Actual Results:**

1. Limitations section expanded successfully.
2. Limitation details and accuracy percentage displayed.
3. Feedback functionality worked correctly.
4. Evidence preview opened with highlighted reference.

---

### TC_022 — Patient Groups Part

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page

**Steps:**

1. Navigate to Template Output part and click the Patient Groups extend button.
2. Capture the screenshot.
3. Click the Add Feedback button.
4. Click the Save button.
5. Click the Edit Feedback button.
6. Click the Show Evidence button.
7. Click the "Open in Preview" button.

**Expected Results:**

1. Patient Groups section shows patient enrollment with match accuracy (%). Add Feedback and Show Evidence buttons are present.
3. Feedback section opens with a text box; user can add feedback.
4. Add Feedback button changes to Edit Feedback button.
5. Previously added comments are present; user can update the existing feedback.
6. Page number is displayed below; Open in Preview button appears.
7. In the right side, the PDF respective page opens and the relevant line is highlighted.

**Actual Results:**

1. Patient Groups section expanded successfully.
2. Patient enrollment details displayed.
3. Feedback saved and edited successfully.
4. Evidence preview displayed correctly.

---

### TC_023 — Study Population Part

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page

**Steps:**

1. Navigate to Template Output part and click the Study Population extend button.
2. Capture the screenshot.
3. Click the Add Feedback button.
4. Click the Save button.
5. Click the Edit Feedback button.
6. Click the Show Evidence button.
7. Click the "Open in Preview" button.

**Expected Results:**

1. Study Result section shows primary outcome with match accuracy (%). Add Feedback and Show Evidence buttons are present.
3. Feedback section opens with a text box; user can add feedback.
4. Add Feedback button changes to Edit Feedback button.
5. Previously added comments are present; user can update the existing feedback.
6. Page number is displayed below; Open in Preview button appears.
7. In the right side, the PDF respective page opens and the relevant line is highlighted.


**Actual Results:**

1. Study Result section expanded successfully.
2. Outcome details displayed with match accuracy.
3. Feedback functionality worked correctly.
4. Evidence preview opened correctly.

---

### TC_024 — Treatment Protocol Part

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page

**Steps:**

1. Navigate to Template Output part and click the Treatment Protocol extend button.
2. Capture the screenshot.
3. Click the Add Feedback button.
4. Click the Save button.
5. Click the Edit Feedback button.
6. Click the Show Evidence button.
7. Click the "Open in Preview" button.

**Expected Results:**

1. Treatment Protocol section shows dosing regimen with match accuracy (%). Add Feedback and Show Evidence buttons are present.
3. Feedback section opens with a text box; user can add feedback.
4. Add Feedback button changes to Edit Feedback button.
5. Previously added comments are present; user can update the existing feedback.
6. Page number is displayed below; Open in Preview button appears.
7. In the right side, the PDF respective page opens and the relevant line is highlighted.

**Actual Results:**

1. Treatment Protocol section expanded successfully.
2. Treatment details displayed with accuracy percentage.
3. Feedback was added and edited successfully.
4. Evidence preview opened correctly.

---

### TC_025 — Validating Existing Uploaded PDF Article Begin Synthesization Flow

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- The PDF already uploaded and result screenshot available to validate

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, click the "Select PDF File" button.
3. Click the Open button.
4. Click the "Begin Synthesization" button.
5. Capture the screenshot.
6. Validate that the details displayed on the Preview page match exactly with the data in the file before upload.

**Expected Results:**

1. User navigated to upload file page.
2. File Explorer opens. Other file types cannot be selected.
3. Selected file name and file size shown. File in "Ready to Process" state. Begin Synthesization and Replace Article buttons are enabled.
4. Verify file is present in S3 path (/PATH). Check T1 - User File Table values compared to existing file data.
6. All details on the Preview page should exactly match the uploaded file data. No data should be missing, altered, or mismatched.

**Actual Results:**

1. File uploaded successfully.
2. Processing workflow executed.
3. Preview page displayed extracted data.
4. Extracted values matched previously uploaded file data.

---

### TC-026 — Navigation Checks Across Pages

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Valid username and password
- URL is accessible

**Steps:**

1. Navigate to the Upload File page and verify the options displayed in the top-right corner.
2. Navigate to the Recent Files page and verify all navigation options in the top-right corner.
3. Navigate to the LuminiAI Portal page and verify all navigation options in the top-right corner.
4. On the Upload File, Recent Files, and LuminiAI Portal pages, click the Back to Home button.
5. From any page, click the Logout button in the top-right corner.

**Expected Results:**

1. Home, Upload File, Recent Files, and LuminiAI Portal options are visible in the top-right corner, along with user email and Logout button.
2. All navigation options, user email, and Logout button are visible. "Recent Files" option is highlighted.
3. All navigation options, user email, and Logout button are visible. "LuminiAI Portal" is highlighted.
4. User is redirected to the Home page.
5. User is successfully logged out and redirected to the login page.

**Actual Results:**

1. Navigation options were visible across pages.
2. Correct tab highlighting was observed.
3. **Back to Home** redirected correctly.
4. Logout worked successfully.

---

### TC-027 — Valid PDF Article Upload and Validating Recent Files View

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Not Executed  
Remarks: 

**Preconditions:**
- Application URL accessible
- Valid Username and Password
- SSO Configuration
- Valid Article file in PDF Format

**Steps:**

1. Navigate to Application URL, enter valid username and password, click Sign In button.
2. In the Recent Files section, click the "View Documents" button.
3. Click the "Open Document" button for any completed document.
4. Capture screenshot.

**Expected Results:**

1. User lands on Takeda login page, navigated to ENTRA SSO; after authentication, lands on the "One Evidence Synthesis Platform" Home Page.
2. User navigated to Recent Documents page. Recently uploaded Manuscript and Oral Presentation documents are listed. Fully completed files have an enabled "Open Document" button; incomplete files show a disabled "Processing" button.
3. User navigated to Preview page showing: PDF, Run ID, Status, Pipeline Status, Structure Summary, Generated XLSX File Name, Overall Progress, Fields Extracted, Quality Score, and Template Output.
4. Screenshot captured.

**Actual Results:**

1. User logged in successfully.
2. Recent Files page displayed uploaded documents.
3. Completed files had **Open Document** enabled.
4. Preview page opened with all expected data.

---

### TC-028 — Lyra Button Validation

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Not Executed  
Remarks: 

**Preconditions:**
- Application URL accessible
- Valid Username and Password
- SSO Configuration
- Valid Article file in PDF Format

**Steps:**

1. Navigate to Application URL, enter valid username and password, click Sign In button.
2. In the Recent Files section, click the "View Documents" button.
3. Click the LYRA button.

**Expected Results:**

1. User lands on Takeda login page, navigated to OKTA SSO; after authentication, lands on the "One Evidence Synthesis Platform" Home Page.
2. User navigated to Recent Documents page. Completed files have an enabled "Open Document" button; incomplete files show a disabled "Processing" button.
3. User is navigated to the LYRA platform.

**Actual Results:**

1. User logged in successfully.
2. Recent Files page opened.
3. Clicking **LYRA button** navigated to LYRA platform successfully.

---

### TC-029 — Validating the Non-GI Therapeutic Area File Upload

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL accessible
- Valid Username and Password
- SSO Configuration enabled
- Non-GI therapeutic area PDF file available in valid PDF format

**Steps:**

1. Navigate to the application URL, enter valid username and password, and click the **Sign In** button.
2. After successful login, navigate to the **Home Page**.
3. Click **Start Processing**.
4. In upload page select the therapetical area and File type
4. Upload the **Non-GI therapeutic area PDF file** using the upload option.
5. Click **Begin Synthesisation** and observe the system behavior.

**Expected Results:**

1. User lands on the Takeda login page, is redirected to **OKTA SSO**, and after successful authentication lands on the **One Evidence Synthesis Platform Home Page**.
2. The system should validate the uploaded file.
3. If the uploaded file belongs to a **Non-GI therapeutic area**, the system should either show an **appropriate validation message** or prevent further processing.
4. The file should **not proceed to synthesization/processing** if the therapeutic area is not supported.

**Actual Results:**

1. User logged in successfully.
2. Non-GI therapeutic file uploaded.
3. System displayed validation message preventing processing.

---

### TC-030 — Validating Large File Upload Scenario

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL accessible
- Valid Username and Password
- SSO Configuration enabled
- Large PDF file available (near or above the supported file size limit)

**Steps:**

1. Navigate to the application URL, enter valid username and password, and click the **Sign In** button.
2. After successful login, navigate to the **Home Page**.
3. Click **Start Processing**.
4. Upload a **large PDF file** using the upload option.
5. Click **Upload / Begin Processing**.
6. Observe the system behavior during file upload and processing.

**Expected Results:**

1. User lands on the Takeda login page, is redirected to **Entra SSO**, and after successful authentication lands on the **One Evidence Synthesis Platform Home Page**.
2. The system should allow upload if the file size is within the supported limit.
3. The system should display a **validation or error message** if the file size exceeds the supported limit.
4. The application should **handle the large file without crashing or performance issues**.
5. Upload status should be clearly displayed to the user (Uploading / Processing / Failed / Completed).

**Actual Results:**

1. Large file upload initiated successfully.
2. System handled upload without crash.
3. Upload and processing status displayed correctly.

---

### TC-031 — Validating Duplicate File Upload While First File is in Processing

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected  

**Preconditions:**
- Application URL accessible
- Valid Username and Password
- SSO Configuration enabled
- Valid GI therapeutic area PDF file available
- File upload and processing functionality is working

**Steps:**

1. Navigate to the application URL, enter valid username and password, and click the **Sign In** button.
2. After successful login, navigate to the **Home Page**.
3. Click **Start Processing**.
4. Upload a valid **PDF file** and start the processing.
5. While the first file is still in **Processing** status, upload the **same PDF file again**.
6. Observe whether the system allows the second file to be uploaded and processed.
7. Once both files are processed, verify the **extracted data** from both uploads.

**Expected Results:**

1. User lands on the Takeda login page, is redirected to **OKTA SSO**, and after successful authentication lands on the **One Evidence Synthesis Platform Home Page**.
2. The system should allow the **same file to be uploaded again** even if the first upload is still in **Processing** status.
3. The second file should also **enter the processing workflow independently**.
4. The system should properly **fetch and extract data for both files**.
5. The **extracted data for both uploads should be identical** since the source file is the same.
6. Both files should be visible in the **Recent Files / Processing list with their respective statuses**.

**Actual Results:**

1. First file entered processing state.
2. Same file uploaded again while processing.
3. Both uploads processed independently.
4. Extracted data for both uploads matched successfully.

---
#### TC_032 — Validate Download Full Files Functionality

**Execution Details:**  
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected 

**Preconditions:**
- User is logged into the NOMI application
- Valid PDF file is available for upload

**Steps:**

1. Log in to the NOMI application.
2. Navigate to the **Upload PDF** page.
3. Upload a valid PDF file.
4. Click on **Begin Synthesization**.
5. Wait until the processing is completed.
6. Navigate to the **Preview Page**.
7. Scroll to the bottom of the page.
8. Click on the **Download Full Files** button.

**Expected Results:**

1. File processing completes successfully and Preview Page is displayed.
2. On clicking the **Download Full Files** button, an **XLSX file** is downloaded.
3. The downloaded file contains the following sheets:
   - study_info
   - chart_data
   - chart_study_metadata
   - patient_characteristics

**Actual Results:**

1. File processing was completed successfully and the Preview Page was displayed.
2. On clicking the **Download Full Files** button, an **XLSX file** was downloaded successfully.
3. The downloaded file contained the following sheets:
   - study_info
   - chart_data
   - chart_study_metadata
   - patient_characteristics

   ---

   #### TC_033 — Validate Publish for Visualization Functionality

**Execution Details:** 
Execution Date: 16-Mar-2026  
Executed By: Dinesh Subramaniyan  
Build Version:  
Status: Pass  
Remarks: Working as expected 

**Preconditions:**
- User is logged into the NOMI application
- Valid PDF file is available for upload

**Steps:**

1. Log in to the NOMI application.
2. Navigate to the **Upload PDF** page.
3. Upload a valid PDF file.
4. Click on **Begin Synthesization**.
5. Wait until the processing is completed.
6. Navigate to the **Preview Page**.
7. On the top-right corner, click the **Publish for Visualization** button.

**Expected Results:**

1. File processing completes successfully and the Preview Page is displayed.
2. The **Publish for Visualization** button is visible on the top-right corner.
3. On clicking the button, the system successfully publishes the file for visualization.
4. A success popup is displayed with the message:  
   **"Files have been published for visualization successfully."**

**Actual Results:**

1. File processing was completed successfully and the Preview Page was displayed.
2. The **Publish for Visualization** button was visible on the top-right corner.
3. On clicking the button, the system successfully published the file for visualization.
4. A success popup was displayed with the message:  
   **"Files have been published for visualization successfully."**