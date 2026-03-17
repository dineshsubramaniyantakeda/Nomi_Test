# Nomi Test Cases

---

## Scenario: User Login Verification

---

### TC_001 — Validating Valid Username and Password login

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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

---

### TC_002 — Validate Login with Valid Username and Empty Password

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC_003 — Validate Login with Valid Username and Invalid Password

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:  

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


---

### TC_004 — Validate User Accessing the NOMI Application from a Non-Takeda Environment

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

**Preconditions:**
- Application URL is accessible
- User is accessing the application from a non-Takeda environment

**Steps:**

1. Navigate to the Application URL.

**Expected Results:**

1. User receives a **"Site can't be reached"** error message.
2. User is unable to access the NOMI application.

**Actual Results:**


---


### TC_005 — Validate Login Attempt Without Entering Username

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC_006 — Validate Error Message for Invalid Email Domain

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC_007 — Validate Error Message for Invalid Username with Correct Domain

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

## Scenario: Validating the Home Page

---

### TC_008 — Validate the Home Page

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

## Scenario: File Upload Through Select PDF File

---

### TC_009 — Validate Valid PDF Upload Through File Browser



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


---

### TC_010 — Validate Invalid File Upload Through File Browser

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

## Scenario: Drag and Drop File Upload

### TC_011 — Validate Valid File Drag-and-Drop Upload

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC_012 — Validate Invalid PDF File Through Drag-and-Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC_013 — Validate Invalid File (XLSX) Format Through Drag-and-Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC_014 — Validate Invalid File (DOC) Format Through Drag-and-Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC_015 — Validate Invalid File (CSV) Format Through Drag-and-Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:  

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



---

### TC_016 — Validating Valid PDF Article Upload and Replace Article

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC_017 — Validating the Valid PDF Article Begin Synthesization Flow

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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
4. Process takes more than 4 seconds. File extraction starts. Verify file is present in S3 path (/PATH). Check values in: T1 - User File Table, T2 - Extraction & Mapping, T3 - Metadata Table, T4 - Template Table, T5 - Curated Output Table. System navigates to Document Processing page (Uploading → Processing pages → Extracting template data → Finalizing). On completion, user is navigated to Preview page.
6. Preview page displays: Run ID, Status, Pipeline Status, Structure Summary, Generated XLSX File Name, Overall Progress (%), Fields Extracted, Quality Score, Template Output Details. Hide PDF and Publish to Lyra buttons are enabled.

**Actual Results:**



---

### TC_018 — Validating Structure Summary for 1st time upload PDF

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

**Preconditions:**
- Complete till valid PDF article upload step
- User will be on PDF Preview page

**Steps:**

1. Navigate to the Structure Summary part and click the extend icon. Validate the details present there.
2. Capture the screenshot.

**Expected Results:**

1. Structure Summary extends showing: Total Pages, Total Headings, Total Tables, Total Figures, Total Text Blocks, Mapped Percentage. Validate counts against the PDF.


**Actual Results:**



---

### TC_019 — Validating Structure Summary for same pdf reupload

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC_020 — Study Overview Part

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:  

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



---

### TC_021 — Outcomes and Evidance

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC_022 — Patient Groups Part

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC_023 — Study Population Part

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC_024 — Treatment Protocol Part

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC_025 — Validating Existing Uploaded PDF Article Begin Synthesization Flow

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC-026 — Navigation Checks Across Pages

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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


---

### TC-027 — Valid PDF Article Upload and Validating Recent Files View

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
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



---

### TC-028 — Lyra Button Validation

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
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



---

### TC-029 — Validating the Non-GI Therapeutic Area File Upload

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC-030 — Validating Large File Upload Scenario

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks: 

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



---

### TC-031 — Validating Duplicate File Upload While First File is in Processing

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:  

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


---

#### TC_033 — Validate Download Full Files Functionality

**Execution Details:**

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