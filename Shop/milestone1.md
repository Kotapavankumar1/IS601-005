<table><tr><td> <em>Assignment: </em> IS601 Milestone1 Deliverable</td></tr>
<tr><td> <em>Student: </em> Pavan Kumar Kota Ravi (pk639)</td></tr>
<tr><td> <em>Generated: </em> 12/12/2022 9:05:40 PM</td></tr>
<tr><td> <em>Grading Link: </em> <a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-milestone1-deliverable/grade/pk639" target="_blank">Grading</a></td></tr></table>
<table><tr><td> <em>Instructions: </em> <ol><li>Checkout Milestone1 branch</li><li>Create a milestone1.md file in your Project folder</li><li>Git add/commit/push this empty file to Milestone1 (you'll need the link later)</li><li>Ensure your images display correctly in the sample markdown at the bottom</li><ol><li>NOTE: You may want to try to capture as much checklist evidence in your screenshots as possible, you do not need individual screenshots and are recommended to combine things when possible. Also, some screenshots may be reused if applicable.</li></ol><li>Save the submission items</li><li>Copy/paste the markdown from the "Copy markdown to clipboard link" or via the download button</li><li>Paste the code into the milestone1.md file or overwrite the file</li><li>Git add/commit/push the md file to Milestone1</li><li>Double check the images load when viewing the markdown file (points will be lost for invalid/non-loading images)</li><li>Make a pull request from Milestone1 to dev and merge it (resolve any conflicts)<ol><li>Make sure everything looks ok on heroku dev</li></ol></li><li>Make a pull request from dev to prod (resolve any conflicts)<ol><li>Make sure everything looks ok on heroku prod</li></ol></li><li>Submit the direct link from github prod branch to the milestone1.md file (no other links will be accepted and will result in 0)</li></ol></td></tr></table>
<table><tr><td> <em>Deliverable 1: </em> Feature: User will be able to register a new account </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add one or more screenshots of the application showing the form and validation errors per the feature requirements</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207139227-7f4d01c0-d4b4-4589-9659-99da6d4bb1ad.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>invalid email and password<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207140150-e16cce65-8177-4642-817d-b2e9d5467c1e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>password not matching validation<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207141412-9b06104a-35d2-4df0-bbed-38b4bd28e455.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Showing email not available validation (already registered)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207141685-39a17b97-6701-4920-8a3f-c619deaca241.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Showing username not available validation (username is taken)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207142104-495bf904-443b-46ef-bb18-85cbb8bddbe7.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Showing the form with valid data filled in before the form is submitted<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot of the Users table with data in it</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207169209-e55fa8e0-6e7c-4430-b0f6-a370c982f8a0.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>user table<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add the related pull request(s) for this feature</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Explain briefly how the process/code works</td></tr>
<tr><td> <em>Response:</em> <div>1.Wtforms is used to handle the form, and each field has its own<br>validation. The form can only be successfully submitted once all of the required<br>fields have been completed.</div><div>2. Validation is performed using Wiforms validators, which work on<br>both the frontend and the backend. The validators listed below are used: DataRequired<br>is used to indicate that a field is required, EqualTo is used to<br>determine whether the password and confirm-password match, and Email is used to validate<br>email format. The username is validated against **(a-20-9_-] (2,30)S" is the regex. Duplicate<br>username and email values are checked during database inserting. For a duplicate entry<br>exception, a flash message is generated.</div><div>3. The password is hashed with barypt before<br>being saved in the database.</div><div>4. All form data is saved in the database<br>in the users table, along with the created and modified timestamps.<br></div><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 2: </em> Feature: User will be able to login to their account </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add one or more screenshots of the application showing the form and validation errors per the feature requirements</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207145466-70f89df0-91c5-43d1-90b3-897cd754124d.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>password mismatch<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207145931-52b1b454-f50c-4207-b09f-71688d9b5a4e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>invalid username<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot of successful login</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207184493-e941c7fb-e605-4612-af90-01d8240a7cad.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>successful login<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207198689-50813891-f2c7-4f72-be53-0a88e7953696.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>successful logout<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add the related pull request(s) for this feature</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Explain briefly how the process/code works</td></tr>
<tr><td> <em>Response:</em> <div><ol><li>Wtforms is used to handle the form, and each field has its own<br>validation. The form can only be successfully submitted once all of the required<br>fields have been completed.</li><li>Validation is performed using wtforms validators, which work on both<br>the front and back ends. The "Email or Username" field accepts either email<br>or username as input and validates it. If the username or email address<br>is not found in the database, a "Invalid User" message is displayed. If<br>the username matches but not the password, a "Invalid Password" message is displayed.&nbsp;</li><li>The<br>entered password is compared to a hashed password already in the database. This<br>matching is performed by the function berypt.check password hash) with the help of<br>the salt value.</li><li>When registering, the database tuples from the users table, which contains<br>the data, are compared with the password and email or username.<br></li></ol></div><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 3: </em> Feat: Users will be able to logout </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot showing the successful logout message</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207147945-f0666c2d-f788-432a-967e-ceae2a872709.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>successfully logged out<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot showing the logged out user can't access a login-protected page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207148170-f67f8d20-e4ac-4591-8cc8-632b0caca279.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>showing the logged out user can&#39;t access a login-protected page<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add the related pull request(s) for this feature</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Explain briefly how the process/code works</td></tr>
<tr><td> <em>Response:</em> <p>when the user logins, the user object is stored in the session.Instead of<br>calling the database, when the page reloads, the User object in the session<br>is used to authenticate. This aids in avoiding overhead.if the user object is<br>not present in the session then it loads from the database.<br></p><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 4: </em> Feature: Basic Security Rules Implemented / Basic Roles Implemented </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot showing the logged out user can't access a login-protected page (may be the same as similar request)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207174254-af2de297-9231-44eb-bccb-7acec9806a6d.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>showing the logged out user can&#39;t access a login-protected page (may be the<br>same as similar request)<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot showing a user without an appropriate role can't access the role-protected page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207175962-4b37c3f9-ae35-4b34-985a-9015e9a6ce2f.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing a user without an appropriate role can&#39;t access the role-protected page<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add a screenshot of the Roles table with valid data</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207170403-dc55d318-8bbf-47ee-a43e-268d8c90f184.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Roles table with valid data<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add a screenshot of the UserRoles table with valid data</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207185913-91760a96-c86d-4072-af8b-e58b92b6915b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>UserRoles table,my admin  is with user pavankumar<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 5: </em> Add the related pull request(s) for these features</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 6: </em> Explain briefly how the process/code works for login-protected pages</td></tr>
<tr><td> <em>Response:</em> <p>The @login required decorator provided by flask_ login protects login-protected pages. For each<br>page request, the user loader is invoked. To avoid repeated database calls, the<br>user will be loaded from the session if it exists. If the session<br>is empty, it loads from the database.<br></p><br></td></tr>
<tr><td> <em>Sub-Task 7: </em> Explain briefly how the process/code works for role-protected pages</td></tr>
<tr><td> <em>Response:</em> <div>Flask principal is used to protect role-protected pages. We define permission in terms<br>of the role required for it. By preceding it with the permission decorators,<br>this permission can be imposed on the desired pages.</div><div>With the user name and<br>authentication type, the identity is loaded into the session.</div><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 5: </em> Feature: Site should have basic styles/theme applied; everything should be styled </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshots to show examples of your site's styles/theme</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207199124-64ef70fc-ae5d-4a43-860e-34f61be181dd.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>styled navigation and styled forms<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207183419-18022696-b503-4b38-b971-9efc7bc26bac.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>styles of table<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add the related pull request(s) for this feature</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 3: </em> Briefly explain your CSS at a high level</td></tr>
<tr><td> <em>Response:</em> <p>I have followed a dark theme for the website. Chose a sample Navigation<br>from the bootstrap where the login, register, and log out will be to<br>the right extreme separated from the main nav. Have chosen a card layout<br>for all the forms with limited width so that the text fields will<br>be within the required length. Have given some inline styles to order the<br>filter and apply the roles layout. Applied custom colors through inline styling<br></p><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 6: </em> Feature: Any output messages/errors should be "user friendly" </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshots of some examples of errors/messages</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207175962-4b37c3f9-ae35-4b34-985a-9015e9a6ce2f.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>permission denied<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207178441-dcc2f0bf-2c99-42a1-9a16-f0cb496556a3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>showing that logged out user cant access to the login protected page<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207141412-9b06104a-35d2-4df0-bbed-38b4bd28e455.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>the choosen email is not available<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207199361-0b977d08-f287-4c70-a0cf-c8b857a6e151.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>page not found<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a related pull request</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 3: </em> Briefly explain how you made messages user friendly</td></tr>
<tr><td> <em>Response:</em> <p>I&#39;ve created separate pages with custom and user-friendly messages for HTTP server error<br>messages like 401, 403, and 404. If any of these errors occur, the<br>browser will be redirected to the appropriate HTML page. I extracted the field<br>name from the exception message and displayed a flash message that it is<br>not available for duplicate entry exceptions that occur for username or email.<br></p><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 7: </em> Feature: Users will be able to see their profile </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshots of the User Profile page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207188332-eaf546d6-520c-455a-b107-ceb7f16d1199.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshots of the User Profile page<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add the related pull request(s) for this feature</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 3: </em> Explain briefly how the process/code works (view only)</td></tr>
<tr><td> <em>Response:</em> <p>The user id is retrieved from the current user when the profile page<br>is loaded. With that user id, the email and username of that user<br>are retrieved from the database and entered into the appropriate fields.<br></p><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 8: </em> Feature: User will be able to edit their profile </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshots of the User Profile page validation messages and success messages</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207196921-34892f88-1d55-45a9-963c-ef8ef423e2e3.png"/></td></tr>
<tr><td> <em>Caption:</em> <p> username and email validation<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207197217-99127ff0-4341-4434-be17-9bfd8e9cdf37.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>password validation<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207197296-24a82914-39a1-460f-8f46-a339868c6d47.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>password mismatch<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207197460-78f6579f-60fb-47c7-ae74-6d1d3b2d117f.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>username already in use<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207197623-f16a2339-ff61-4be5-9c72-1a0d60f1d6ef.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>chosen email is already in use<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add before and after screenshots of the Users table when a user edits their profile</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207197934-8267fe71-907f-4053-8d79-761a42d13577.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>user table before changes<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207198054-5ba93894-aca9-42c8-896e-d6627c3bddb7.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>changed username<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/207198218-40a9eca9-e3ea-4a02-9acf-5c69b9234663.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>user table after changes<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add the related pull request(s) for this feature</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/17">https://github.com/Kotapavankumar1/IS601-005/pull/17</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Explain briefly how the process/code works (edit only)</td></tr>
<tr><td> <em>Response:</em> <p>For each update request, the username and email fields are updated. They checked<br>if the username and email values were in the correct format before updating<br>them. If yes, it checks to see if either of the values is<br>already in use by another user in the database. If yes, a flash<br>message is displayed informing the user that the specified value is not available<br>for use. To update the password, we first check to see if the<br>new password matches the confirm password, and then we see if the current<br>password matches the existing password in the database. If these conditions are met,<br>the password is changed.<br></p><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 9: </em> Misc </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Describe any issues and learnings throughout this milestone</td></tr>
<tr><td> <em>Response:</em> <div><ul><li>I've encountered jinja2.exceptions. UndefinedError. 'flask login.mixins. AnonymousUserMixin object has no attribute 'has role"<br>It was discovered that the problem was caused by my checking for the<br>current user before checking if the user was authenticated. It was fixed by<br>including an authentication check before checking the role.</li><li>&nbsp;Tried to populate the wtforms with<br>form.process, but discovered that the User object cannot be iterated. As a result,<br>I reverted to the convention assigning approach.</li></ul></div><br></td></tr>
<tr><td> <em>Sub-Task 2: </em> Prod Application Link to Login Page</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/login">https://is601-pk639-prod-2.herokuapp.com/login</a> </td></tr>
</table></td></tr>
<table><tr><td><em>Grading Link: </em><a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-milestone1-deliverable/grade/pk639" target="_blank">Grading</a></td></tr></table>