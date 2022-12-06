<table><tr><td> <em>Assignment: </em> IS601 Mini Project 2  Business Management</td></tr>
<tr><td> <em>Student: </em> Pavan Kumar Kota Ravi (pk639)</td></tr>
<tr><td> <em>Generated: </em> 12/5/2022 10:52:35 PM</td></tr>
<tr><td> <em>Grading Link: </em> <a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-mini-project-2-business-management/grade/pk639" target="_blank">Grading</a></td></tr></table>
<table><tr><td> <em>Instructions: </em> <ol><li>checkout dev and pull any latest changes</li><li>Create a branch called MiniProject-2</li><li>Add all the baseline files first under a folder called BusinessManagement (included below)</li><li>Don't forget to copy your .env file from flask_sample into BusinessManagement</li><li>source the venv and pip install the requirements.txt</li><li>Run the BusinessManagement/sql/init_db.py script</li><li>Immediate add/commit/push to github</li><li>Open a pull request and keep it open until you're done adding the submission file</li><li>&nbsp;(optional) updated the deploy dev yml file and add MiniProject-2 so you can deploy to dev without needing to merge into dev</li><li>Make your code changes per the following requirements</li><ol><li>Important: run the test files indiviudally as you're working/testing to save on query quota usage</li></ol><li>Add/commit periodically (recommended after you implement a TODO item or checlist item)<br></li><li>Anywhere relevant add your ucid and the date you added the code (best to do this as you go)</li><li>You'll be capturing website screenshots from dev and code snippet screenshots (ensure you upload these properly as pull request comments to the pull request from step 5</li><ol><li>Note: You don't need separate screenshots for each checklist item, when possible it's recommended to try to capture multiple items together</li><li>Ensure all screenshots are properly captioned in the deliverable section</li></ol><li>You may save your progress when filling out this submission as often as you want</li><li>Once done, copy the markdown or download the md file and save it under the BusinessManagement folder</li><li>Do a final add/commit/push</li><li>Verify everything looks ok in the pull request</li><li>Merge the pull request</li><li>Make a new pull request from dev to prod and merge it</li><li>Navigate to the submission file under the BusinessManagement folder</li><li>Copy the github url to the exact file and submit it to Canvas</li></ol><div>You'll be implementing a basic Business Management site.</div><div>There will be some provided files fully working as-is and some skeleton files you'll need to fill in.</div><div>The files you need to fill in will have TODO items or comments mentioning what's expected.</div><div>There are provided test case files too that all must be passing for full credit. Do not edit these test case files.</div><div>The site will handle CRUD operations for Companies and Employees as well as allowing import of Company/Employee data via a csv file.</div><div><br></div><div>Baseline files:&nbsp;<a href="https://github.com/MattToegel/IS601/tree/F22-MiniProject-2">https://github.com/MattToegel/IS601/tree/F22-MiniProject-2</a></div><div>May want to download branch as a zip, then copy/paste the files into your repo</div><div><br></div><div>Provided files you don't need to edit:</div><div><ul><li>000_create_table_companies.sql</li><li>001_create_table_employees.sql</li><li>db.py</li><li>init_db.py</li><li>flash.html</li><li>company_dropdown.html</li><li>country_state_selector.html</li><li>upload.html</li><li>sort_filter.html</li><li>all test files</li><li>geography.py</li><li>__init__.py (remains empty)</li><li>Dockerfile</li><li>main.py</li><li>index.py</li></ul><div>All other files likely have requirements to fill in.</div></div><div><br></div></td></tr></table>
<table><tr><td> <em>Deliverable 1: </em> Identity Edits and Setup </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshot of the index page being displayed (from dev)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205558884-ec6cc682-8ac4-4387-86f2-f985ac5210c3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>DIAR-mt85 should be updated to DIAR-ucid of the student (in loayout.html)<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add screenshot from the DB extension of vs code / IDE</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205791886-1eff4611-9817-4b01-90bf-c6c9e5e86078.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>company table<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205792082-c2191c86-7f95-43e3-9547-c3725495bd86.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>employee table<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 2: </em> Upload / Import CSV File (provided data.csv) </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshot of /import route</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205540943-3e6d50e7-0ffb-4c75-aaba-7e773d6dfe64.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Code should check if the file is a .csv file<br>otherwise reject with a flash<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205541442-6208246b-c9ae-49c1-97b3-ee6b5a5b3688.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for CSV file should be read from the provided stream as<br>a dict<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205541596-37ebd3ae-51d5-4a7d-a365-6194948c8174.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Extracted employee data should be append as a dict to<br>the employee list<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205541788-ecf1fa67-aed7-496f-bd46-a429fb482dcf.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Extracted company data should be appneded as a dict to<br>the comapny list<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205542113-1b2eacd8-3ced-4d7c-b7a5-b93ec8ba82f8.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for After each query a flash message should be generated noting<br>how many records were processed<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205542421-e4d53efc-2f6a-4d3f-9062-a11dfa98ee6a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for If a particular list was empty a flash message should<br>note that the particular list wasn&#39;t loaded or was empty<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Screenshots of the website when uploading the data.csv file</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205792449-15476d61-6127-4250-817b-04311c535a0b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Show the error message when the file is not a .csv file<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205792996-aeb8e1d2-7e1b-406b-bb57-f5d052cb8531.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing how many successful records are processed on asuccessful  cv file<br>upload<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205793143-034888d5-18ea-42e4-9ace-0a51ac0bcefc.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing the error message when the form was submitted without a file<br>attached<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Screenshots of DB data (basic summary/view)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205790793-1dbd3b6e-fbaf-459e-a311-a86c850978e6.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>employee data<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205791273-f9b8ce04-0a3c-4604-8f18-34a525244b2a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>company data<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 3: </em> Add Employee </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot of code for /add route of employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205542952-2d769ee5-681e-4e6e-90f0-ff62920fd72e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Code should retrieve first_name, last_name, company (id), email<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205543352-355e9133-ec20-4e49-99f2-8f85d7bf2b4c.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for first_name is required (flash proper error message), last_name is required<br>(flash proper error message), company doesn&#39;t require a flash and may be empty/None,<br>email is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205543485-9c6af0a7-d6e9-4d45-9684-d20adca6ae4d.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>added code for Proper INSERT query should be visible, Except block should have<br>a user friendly message flashed and a print() of the exception<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Screenshots of website for add employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205793564-5953f3fd-227c-47b1-8233-41e51547c265.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>add employee form-filled in valid data prior to submission<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205793837-0ce53a86-2474-4c36-86eb-2722c25b1ae8.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>success flash message for adding employee record<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205567869-36fd6bd5-8ca8-49de-81c8-134edc338aa3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>first name error message<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205568946-1f7046a5-7862-4997-b769-534e06bd1fa7.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>last name error message<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205569452-f4bd9c36-2ae7-41e4-af22-ddadbc1a53c4.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>email error message<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Screenshot of new employee DB record from VS Code / IDE</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205791458-80575a0c-9bae-4da4-85b4-439a9ec7fca1.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>new employee DB record from vs code highlighting the newly added employee record<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 4: </em> List/search Employees </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshots of code for /search route of employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205544155-1cc325c1-9dd9-402c-b6fb-a60e9583297a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for SELECT query should be filled in properly to pull employ<br>id, first_name, last_name, email, company_id, company_name via a LEFT JOIN<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205544270-3ab47e99-db2d-4551-a3de-677f13d29e8d.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Check request args for fn, ln, email, company, column, order,<br>limit (exact naming is required)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205544356-48ea0b81-55df-4c1f-9ed6-aab2862be278.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for append like filter for first_name if provided, append like filter<br>for last_name if provided, append like filter for email if provided<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205544441-39a39bcd-d2af-405e-95a9-e0e63e7bc131.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for append equality filter for company_id if provided, append sorting if<br>column and order are provided and within the allowed columns and order options<br>(asc, desc) allowed_columns = [&quot;first_name&quot;, &quot;last_name&quot;, &quot;email&quot;, &quot;company_name&quot;]<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205544637-b663671e-5f5b-4b53-be8d-195be0a86c7b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for append limit (default 10) or limit greater than 1 and<br>less than or equal to 100<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205544823-3c2dc20e-fbfd-4025-92e9-e17251aed48d.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for provide a proper error message if limit isn&#39;t a number<br>or if it&#39;s out of bounds<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205544911-bb9a3208-3945-4086-850c-986f3046af83.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Except block should have a user friendly message flashed and<br>a print() of the exception<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Screenshots of website for search employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205571940-6ee2b824-7300-4adc-b89f-8cf959734737.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>first name filter<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205794108-4960af61-b2e4-45e2-9be1-cfacbc43b2f7.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>last name filter<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205573336-636a06e8-0b25-45c5-a29f-a17448fe1baa.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>email filter<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205573707-cb9b0466-6029-49db-84aa-846d40c7a807.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>company filter<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205578350-09233e71-55f7-4187-920b-b52dcbe42854.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>ascending order<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205578568-771423a0-3165-4338-9998-4396ce7085a7.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>descending order<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 5: </em> Edit Employee </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshots of code for /edit route of employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205545346-08e3af46-4c43-4586-8623-23118a3f0153.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Code should retrieve id (from request args) first_name, last_name, company<br>(id), email from form<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205545547-eb87fbe5-a2f4-49ac-9c1e-824f6c54db9c.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for first_name is required (flash proper error message), last_name is required<br>(flash proper error message), company doesn&#39;t require a flash and may be empty/None,<br>email is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205545721-ec33a538-390b-4573-8e11-b8b4fb74246b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Proper UPDATE query should be visible<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205545960-516384bd-bbcb-4f0e-801c-601673f14d88.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Except blocks (two) should have a user friendly message flashed<br>and a print() of the exception<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205546268-e193b97a-2688-4c4d-b189-e1dfa4576944.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Added code for Proper SELECT query should be visible, Employee data should be<br>passed to the render_template()<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Screenshots of website for edit employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205717735-f9573f97-15c4-4b61-a911-18db85b30bc5.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>data before an edit<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205718064-ddbb68e9-b255-4435-8700-43373b053958.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>edit page before edit<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205718662-854edfc5-aa27-45a9-bf03-d41cdd6e4991.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>page of updated employee record after edit<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205719065-c407a65c-a048-421c-afd3-a0ea07f86549.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>updated record<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Screenshots of DB data before and after of employee data edit from VS Code / IDE</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205784994-12c8f9c4-121c-478e-ac2e-b40bccd0ac2b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>DB before editing an email<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205785038-550e2b97-3aca-470e-acd1-bfd60275514d.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>DB after editing an email<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 6: </em> Add company </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot of code for /add route of company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205777648-1bebbdbd-3607-459c-88b7-35a242ac91ee.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>code should retrieve form data for name, address, city, state, country, zip, website<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205777871-94dc1a05-a784-4409-82b6-f32aa3bf8dc8.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>name is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205777871-94dc1a05-a784-4409-82b6-f32aa3bf8dc8.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>address is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205777871-94dc1a05-a784-4409-82b6-f32aa3bf8dc8.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>city is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205778351-66338d17-aa57-4ba7-9196-3d0fe7f5b1b9.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>state is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205778351-66338d17-aa57-4ba7-9196-3d0fe7f5b1b9.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>country is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205778351-66338d17-aa57-4ba7-9196-3d0fe7f5b1b9.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>website is not required<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205778735-7172e17f-2247-4b9a-b5ab-601eea58a865.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Proper INSERT query should be visible and Except block should have a user<br>friendly message flashed and a print() of the exception<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Screenshots of website for add company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205724323-424c9141-effe-46ad-975d-cffaf4de39df.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>filled data prior submission <br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205724709-c366da3b-6925-43eb-9f28-71ad8f823c31.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>successfully added company<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205725032-307a4402-e4ed-4933-a792-25bc1fbd790a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>name error<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205725322-265966c8-ec8b-4d74-9d6d-0613fdb46414.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>address error<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205725562-f7a2172f-28d8-4cf6-a6a6-87454be06959.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>city error<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205725981-8723e205-b7d0-4b6e-b653-aac1392460e6.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>state<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205726181-903dbdb4-5d57-4a7f-b5a0-607a9649690a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>country<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Screenshot of new company DB record from VS Code / IDE</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205782443-fae9c91e-0b88-472d-83c9-2b224ea5c4b1.PNG"/></td></tr>
<tr><td> <em>Caption:</em> <p>AFTER ADDING AN VALID COMPANY<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 7: </em> List/Search Comapny </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshots of code for /search route of company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205546853-0ea1d730-ca80-4d62-b887-cceab2efd5ff.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>code for SELECT query should fetch id, name, address, city, country, state, zip,<br>website, employee count for the company (likely a sub-query is needed)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547016-89bd15bd-83ac-4822-814d-19da64a89584.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>code for Check request args for name, country, state, column, order, limit<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547238-564cc124-77e6-41f4-960d-c0b4b2483ddb.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>append a LIKE filter for name if provided<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547337-a269f349-a261-4e12-adc0-b2998a077a28.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>append an equality filter for country if provided<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547446-d141c80a-f526-439a-b651-e99c16cf2459.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>append an equality filter for state if provided<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547580-07f160a4-68b5-42e6-b92f-fdba086b1997.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>append sorting if column and order are provided and within the allows columsn<br>and allowed order asc,desc allowed_columns = [&quot;name&quot;, &quot;city&quot;, &quot;country&quot;, &quot;state&quot;]<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547580-07f160a4-68b5-42e6-b92f-fdba086b1997.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>append limit (default 10) or limit greater than 1 and less than or<br>equal to 100<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547580-07f160a4-68b5-42e6-b92f-fdba086b1997.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>provide a proper error message if limit isn&#39;t a number or if it&#39;s<br>out of bounds<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205547878-a6759b42-46f7-48ad-baaf-ded9c47ec2d1.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Except block should have a user friendly message flashed and a print() of<br>the exception<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Screenshots of website for search company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205749379-e010fcfa-4c1f-4847-83df-fd4aed7454ae.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>results with name filter applied<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205749905-e0b24595-9eb3-4c63-a451-07733afd1596.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>country filter applied<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205750595-5a03c7e3-864e-4d51-8f21-cd84c87cbfb6.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>state filter applied<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205750900-8d3c0b94-58d3-4c1d-bae1-ccd7e84ebb3b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>asscending order filter applied<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205751352-8c18f52e-69a9-43f4-9628-2969443c2d9f.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>descending filter applied<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 8: </em> Edit Company </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshots of code for /edit route of company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548466-3e15a1dd-e5ed-4d3f-a1d4-c2f03ab51777.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Code should retrieve id (from request args) name, address, city, state, country, zip,<br>website from form<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548542-7314e7ae-3e1b-4b81-9bf1-a4c4ad1de961.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>name is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548662-6c65f641-3706-4285-a2f7-f7964da9f336.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>address is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548662-6c65f641-3706-4285-a2f7-f7964da9f336.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>city is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548662-6c65f641-3706-4285-a2f7-f7964da9f336.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>state is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548662-6c65f641-3706-4285-a2f7-f7964da9f336.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>country is required (flash proper error message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548662-6c65f641-3706-4285-a2f7-f7964da9f336.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Proper UPDATE query should be visible<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548662-6c65f641-3706-4285-a2f7-f7964da9f336.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Except blocks (two) should have a user friendly message flashed and a print()<br>of the exception<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548806-6decef43-f7fe-4b29-aa06-63f0f68f3813.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Proper SELECT query should be visible<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205548806-6decef43-f7fe-4b29-aa06-63f0f68f3813.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Company data should be passed to the render_template()<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Screenshots of website for edit company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205785475-98025c7a-5de6-4410-b78a-f4c51516f03c.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>before an edit<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205785701-5a787791-986b-4ab6-ba66-4e43d4ec8628.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>edit page before editing<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205785879-f1e73fa7-5d50-4917-97b4-a2c2ccfbab39.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>record has been saved<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205786061-2f08e130-731d-4cff-96c5-e986f5af3ceb.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>after editing the city<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Screenshots of DB data before and after of company  data edit from VS Code / IDE</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205794637-c22ac9a4-c119-41c0-a4e7-b81f339975fe.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>before editing chanay company city <br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205794797-bdfd0297-21fc-40d4-aecb-e7e12ac5ecde.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>after editing the chanay city to newyork<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 9: </em> Delete Employee and Delete Company </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot of code for /delete route of employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205549809-fdb97b4b-97b1-4ff5-a2ce-97bb4affe9e3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Delete employee by id<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205549809-fdb97b4b-97b1-4ff5-a2ce-97bb4affe9e3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Redirect to employee search<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205549809-fdb97b4b-97b1-4ff5-a2ce-97bb4affe9e3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>All request args (minus id) are passed to the redirect route<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205549809-fdb97b4b-97b1-4ff5-a2ce-97bb4affe9e3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Success message should be flashed if the process worked<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a before and after website screenshot of deleting an employee</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205787052-7f6d6a04-9c9f-4831-ab6d-c0cd20ca4d1a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>before deleting an employee<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205787265-07ed6b01-f060-4881-b362-1ab7ee58a460.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>delete employee recorded<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205787405-947937b2-d5bf-47ed-80ba-c2c5bebec5bc.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>after deletion<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Screenshot of code for /delete route of company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205550237-e2737d29-546c-4073-a1f8-8415516a866b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Delete company by id<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205550237-e2737d29-546c-4073-a1f8-8415516a866b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Redirect to company search<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205550237-e2737d29-546c-4073-a1f8-8415516a866b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>All request args (minus id) are passed to the redirect route<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205550237-e2737d29-546c-4073-a1f8-8415516a866b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Success message should be flashed if the process worked Preview<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add a before and after website screenshot of deleting a company</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205788622-0b6414f6-bed7-4815-ba67-cd2d9654a9e0.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>before deletion of a company<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205788747-07a0a32d-39bd-4106-88e3-0a3b688696b8.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>deletion recorded<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205788894-c4bb903d-017f-499a-a0e6-83d5e72bb6fc.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>after deletion<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 10: </em> Test Cases and Misc </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot Test case Results</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/205795256-ebbb8925-2f79-43b1-86f6-cc730e1a430c.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>test cases<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Issues / Learnings / Interesting things to note</td></tr>
<tr><td> <em>Response:</em> <p>I have learned the handling of GET and POST requests to carry out<br>operations like edit, sort , and delete. mastered using Wtforms and passing arguments<br>to it and i also learned the handling of exception messages. I had<br>an issue with test cases and also reading data file then I figured<br>it out.<br></p><br></td></tr>
</table></td></tr>
<table><tr><td><em>Grading Link: </em><a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-mini-project-2-business-management/grade/pk639" target="_blank">Grading</a></td></tr></table>