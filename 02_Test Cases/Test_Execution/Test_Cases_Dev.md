# Nomi Test Cases

---

## Sheet 1: Upload File

---

### Scenario: User Login Verification

---

#### TC_001 — Validating Valid Username and Password

**Execution Details:**
Execution Date: 02-Mar-2026
Executed By: Dinesh Subramaniyan
Build Version: V 1.0
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


---

#### TC_002 — Validating valid Username, Empty Password

**Execution Details:**
Execution Date: 02-Mar-2026
Executed By: Dinesh Subramaniyan
Build Version: V 1.0
Status: Pass
Remarks: Working As expected

**Preconditions:**
- Application URL is accessible
- Valid Username 
- User has Entra access

**Steps:**

1. Navigate to the Application URL.
2. Enter an valid username and valid password and click the Sign In button.
3. Capture screenshot with error message.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays "Please Enter Your password" message 

---

#### TC_003 — Validating Valid Username and Invalid Password

**Execution Details:**
Execution Date: 02-Mar-2026
Executed By: Dinesh Subramaniyan
Build Version: V 1.0
Status: Pass
Remarks: Working as expected

**Preconditions:**
- Application URL is accessible
- Valid Username and invalid Password
- User has Entra access

**Steps:**

1. Navigate to the Application URL.
2. Enter a valid username and invalid password and click the Sign In button.
3. Capture screenshot with error message.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays "Your Account or Password is incorrect. If you Dont Remmber your password reset it now" message; user is not logged in and remains on the login page.

---

#### TC_004 — Validating User accessing the NOMI Application from other environment

**Execution Details:**
Execution Date: 02-Mar-2026
Executed By: Dinesh Subramaniyan
Build Version: V 1.0
Status: Pass
Remarks:Working As Expected

**Preconditions:**
- Application URL is accessible
- User is in non takeda environment

**Steps:**

1. Navigate to the Application URL.

**Expected Results:**

1. User getting the site cannot be reach error message

---


#### TC_005 — Validating without user name if user clicks the nect button

**Execution Details:**
Execution Date: 02-Mar-2026
Executed By: Diensh subramaniyan
Build Version: V 1.0
Status: Pass
Remarks:Working As Expected

**Preconditions:**
- Application URL

**Steps:**

1. Navigate to the Application URL.
2. Leave Email Field as Empty click the Next button.
3. Capture screenshot with error message.

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays "Enter a Valid Email address ,Phone number or Skype name" error message; user is not logged in and remains on the login page.

---

#### TC_006 — Validating the error message while entering the invalid domain name in mail address

**Execution Details:**
Execution Date: 02-Mar-2026
Executed By: Diensh subramaniyan
Build Version: V 1.0
Status: Pass
Remarks:Working As Expected

**Preconditions:**
- Application URL
- Invalid email

**Steps:**

1. Navigate to the Application URL.
2. Entering the Invalid domain name email address
3. click Next

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays "We Couldn't find an account with that user name" error message; user is not logged in and remains on the login page.

---

#### TC_007 — Validating the error message while entering the invalid username and correct Domain name

**Execution Details:**
Execution Date: 02-Mar-2026
Executed By: Diensh subramaniyan
Build Version: V 1.0
Status: Pass
Remarks:Working As Expected

**Preconditions:**
- Application URL
- Invalid email

**Steps:**

1. Navigate to the Application URL.
2. Entering the Invalid user name and correct domain name email address
3. click Next

**Expected Results:**

1. User is redirected to the Takeda login page.
2. System displays "The username may be incorrect make sure you typed it correctly otherwise contact your admin" error message; user is not logged in and remains on the login page.



### Scenario: Validating the Home Page

---

#### TC_005 — Validating the Home Page

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

1. Log in to the application and navigate to the Home page. Verify that the Upload File, Recent Files, and LuminiAI Portal options are displayed.
2. Verify that on the Home page, the user email and Logout icon are displayed in the top-right corner.
3. Click the Logout icon.

**Expected Results:**

1. After successful login, Upload File, Recent Files, and LuminiAI Portal options should be visible on the Home page.
2. After successful login, the user email and Logout icon should be visible in the top-right corner.
3. The user should be successfully logged out of the application.

---

### Scenario: File Upload Through Select PDF File

---

#### TC_006 — Validating Valid PDF Upload Through File Browser

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

**Preconditions:**
- Complete user login
- Valid PDF File

**Steps:**

1. On the Takeda Home page, under the Upload File section, click "Start Processing."
2. Validate that the Home, Upload File, Recent Files, and LuminiAI Portal options are displayed in the top-right corner, along with the user email and Logout button.
3. Select Therapeutic Area as GI and Document Type as Manuscript, then click the "Select PDF File" button.
4. In the File Explorer window, choose a PDF file and click "Open."

**Expected Results:**

1. System responds without errors and navigates to the upload page.
2. All navigation options, user email, and Logout button should be visible in the top-right corner.
3. The File Explorer window opens, allowing only PDF files to be selected. Other file formats are not selectable.
4. The selected file name and file size are displayed in the Upload File section. File status shows "Ready to Process." Begin Synthesization and Replace Article buttons are enabled. Capture screenshot.

---

#### TC_007 — Validating Invalid File Through the File Browser

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

**Preconditions:**
- Complete user login
- Invalid PDF File

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, then click the "Select PDF File" button.
3. Click the Open button.
4. Capture the screenshot of the page.

**Expected Results:**

1. User navigated to upload file page.
2. File Explorer opens. Verify that files other than PDF cannot be selected.
3. Check the Error message.

---

### Scenario: Drag and Drop File Upload

---

#### TC_008 — Validating Drag and Drop File Upload

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

**Preconditions:**
- Complete user login
- Valid PDF File

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, then drag and drop the valid PDF file.
3. Capture the screenshot of the page.

**Expected Results:**

1. User navigated to upload file page.
2. Selected file name and file size are displayed. File is in "Ready to Process" state. Begin Synthesization and Replace Article buttons are enabled.

---

#### TC_009 — Validating Invalid PDF File Through Drag and Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

**Preconditions:**
- Complete user login
- Invalid PDF File

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, then drag and drop the invalid PDF file.
3. Capture the screenshot of the page.

**Expected Results:**

1. User navigated to upload file page.
2. Check the Error message.

---

#### TC_0010 — Validating Invalid File (XLSX) Format Through Drag and Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

**Preconditions:**
- Complete the user login step
- Have an invalid format file

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, then drag and drop the invalid format (XLSX) file.
3. Capture the screenshot of the page.

**Expected Results:**

1. User navigated to upload file page.
2. Check the Error message.

---

#### TC_011 — Validating Invalid File (DOC) Format Through Drag and Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

**Preconditions:**
- Complete the user login step
- Have an invalid format file

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, then drag and drop the invalid format (DOC) file.
3. Capture the screenshot of the page.

**Expected Results:**

1. User navigated to upload file page.
2. Check the Error message.

---

#### TC_012 — Validating Invalid File (CSV) Format Through Drag and Drop

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

**Preconditions:**
- Complete the user login step
- Have an invalid format file

**Steps:**

1. In Takeda Home page under upload file section, click "Start Processing."
2. Choose Therapeutic Area as GI, Document Type as Manuscript, then drag and drop the invalid format (CSV) file.
3. Capture the screenshot of the page.

**Expected Results:**

1. User navigated to upload file page.
2. Check the Error message.

---

### Scenario: Replace Article

---

#### TC_013 — Validating Valid PDF Article Upload and Replace Article

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

---

### Scenario: Begin Synthesization

---

#### TC_014 — Validating the Valid PDF Article Begin Synthesization Flow

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

---

### Scenario: Structure Summary Validation

---

#### TC_015 — Validating Structure Summary for New PDF

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

---

#### TC_016 — Validating Structure Summary for Existing Uploaded PDF

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

---

### Scenario: Template Output Validation — Add Feedback and Show Evidence

**Execution Details:**
Execution Date: 
Executed By: 
Build Version: 
Status: 
Remarks:

---

#### TC_017 — Overview Part

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

1. Navigate to Template Output part and click the Overview section extend icon.
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

---

#### TC_018 — Endpoint Definitions Part

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

1. Navigate to Template Output part and click the Endpoint Definitions extend button.
2. Capture the screenshot.
3. Click the Add Feedback button.
4. Click the Save button.
5. Click the Edit Feedback button.
6. Click the Show Evidence button.
7. Click the "Open in Preview" button.

**Expected Results:**

1. Endpoint Definitions section shows the primary endpoint with match accuracy (%). Add Feedback and Show Evidence buttons are present.
3. Feedback section opens with a text box; user can add feedback.
4. Add Feedback button changes to Edit Feedback button.
5. Previously added comments are present; user can update the existing feedback.
6. Page number is displayed below; Open in Preview button appears.
7. In the right side, the PDF respective page opens and the relevant line is highlighted.

---

#### TC_019 — Limitations Part

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

1. Navigate to Template Output part and click the Limitations extend button.
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

---

#### TC_020 — Patient Groups Part

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

---

#### TC_021 — Study Result Part

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

1. Navigate to Template Output part and click the Study Result extend button.
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

---

#### TC_022 — Treatment Protocol Part

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

---

#### TC_023 — Validating Existing Uploaded PDF Article Begin Synthesization Flow

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

---

### Scenario: Navigation Checks

---

#### TC-024 — Navigation Checks Across Pages

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

---

## Sheet 2: Recent File

---

### Test Case — Valid PDF Article Upload and Validating Recent Files View

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

1. User lands on Takeda login page, navigated to OKTA SSO; after authentication, lands on the "One Evidence Synthesis Platform" Home Page.
2. User navigated to Recent Documents page. Recently uploaded Manuscript and Oral Presentation documents are listed. Fully completed files have an enabled "Open Document" button; incomplete files show a disabled "Processing" button.
3. User navigated to Preview page showing: PDF, Run ID, Status, Pipeline Status, Structure Summary, Generated XLSX File Name, Overall Progress, Fields Extracted, Quality Score, and Template Output.
4. Screenshot captured.

---

### Test Case — Lyra Button Validation

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

---

*Sheet 3: LuminiAI — No test cases recorded.*

