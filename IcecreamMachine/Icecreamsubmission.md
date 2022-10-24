<table><tr><td> <em>Assignment: </em> IS601 - Mini Project 1 - IceCream</td></tr>
<tr><td> <em>Student: </em> Pavan Kumar Kota Ravi (pk639)</td></tr>
<tr><td> <em>Generated: </em> 10/23/2022 9:59:42 PM</td></tr>
<tr><td> <em>Grading Link: </em> <a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-mini-project-1-icecream/grade/pk639" target="_blank">Grading</a></td></tr></table>
<table><tr><td> <em>Instructions: </em> <ol><li>Create a new branch per the desired branch name below</li><li>Add the baseline files from the following link:&nbsp;<a href="https://gist.github.com/MattToegel/17d0ac833a03580d010ad92e83fc4216">https://gist.github.com/MattToegel/17d0ac833a03580d010ad92e83fc4216</a>&nbsp;</li><li>Put them into a subfolder in your repository folder (I called my folder IcecreamMachine)</li><li>git add .</li><li>git commit -m "baseline files"</li><li>git push origin (name of desired branch below)</li><li>You can go to github and open the pull request for evidence capturing later (don't close/merge the pull request until you're done with the assignment)</li><li>Do the below tasks and fill in the below entries</li><ol><li>git add/commit after any significant changes to build up history</li></ol><li>Save the input and generate the submission markdown file (copy to clipboard or download the file)</li><li>Name it something relevant to the assignment if it's not named already</li><li>git add the submission file</li><li>git commit the submission file</li><li>git push the submission file</li><li>Complete the pull request to dev</li><li>Create a pull request from dev to prod</li><li>Go to the prod branch on github, navigate to the submission file</li><li>Paste that link to Canvas</li></ol></td></tr></table>
<table><tr><td> <em>Deliverable 1: </em> Code Changes - Add the calculate_cost() implementation </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot(s) of the updated method calculate_cost()</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197422576-20abdae0-7d99-4acd-9419-d94ce69028d3.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>code for calculating the cost <br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197422671-c9a342fe-c89f-4b96-bf84-9c74ac6807b8.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>output of the icecream machine calculating cost<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Explain the approach to implementing the calculation</td></tr>
<tr><td> <em>Response:</em> <p>Firstly we initialize the cost with 0&nbsp;<div>The in-progress ice cream array is iterated<br>over to add the cost of each choice by using for loop</div><div>then we<br>return the cost by formatting the currency&nbsp; to decimal points by using :.2f.format()<br>function</div><div><br></div><br></p><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 2: </em> Exception Handling </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot(s) of adjusted code to handle exceptions</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197423598-018dec3d-fc3b-4fe8-af02-8b7a7f2cab29.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>OutOfStockException is handled in this screenshot<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197423937-1597178b-2ccc-4279-8b88-b382ca635ec1.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>NeedsCleaningException is handled <br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197430459-98d3ee04-650d-4687-b07a-25aefcf74293.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p> InvalidChoiceExceptions are handled <br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197423751-1af40b81-0ef6-4ef4-b5ea-87d76c1b12f1.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>ExceededRemainingChoicesExceptions<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197424039-1c0fc1bf-67f9-49f1-9ecd-547ceb374872.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p> InvalidPaymentException<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Summarize each exception handling process</td></tr>
<tr><td> <em>Response:</em> <p><span style="font-size: 13px;">OutOfStockException:&nbsp;If a user-chosen item is out of stock, this exception kicks<br>in and outputs the message &quot;The item you have choosen is out of<br>stock, please select another item.&quot;</span><div><span style="font-size: 13px;">NeedsCleaningException: This exception will output &quot;Machine should<br>be clean for further usage&quot; when an ice cream machine is used multiple<br>times and has to be cleaned before the next use.</span></div><div><span style="font-size: 13px;">InvalidChoiceException:&nbsp;When a<br>user enters an incorrect word, this exception will print &quot;you entered option please<br>pick a valid option.&quot;</span></div><div><span style="font-size: 13px;">ExceededRemainingChoicesException: The message &quot;Your maximum scoops have been<br>attained please pick toppings&quot; appears when the number of scoops reaches its limit.<br></span></div><div>&lt;span<br>style=&quot;font-size: 13px;&quot;&gt;InvalidPaymentException:&nbsp;The message &quot;The amount you provided is mismatched therefore please input exact<br>amount&quot; is shown when the user&#39;s entry is in error.<br></span></div><br></p><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 3: </em> Test Cases </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot(s) of test cases per the checklist</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197425770-a7884150-320c-4071-8c0f-a717b6fd4ca1.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>test1:containers must be first selection<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197425906-86fba635-7374-4667-8d00-ba6f9f61069a.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>Test 2 - can only add flavors if they&#39;re in stock<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197425925-5a77b505-e2fc-430b-abc8-59e454b8c157.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>Test 3 - can only add toppings if they&#39;re in stock<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197426116-85454f06-35db-418a-a83c-b46e9e158fa2.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>Test 4 - Can add up to 3 flavors/scoops<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197426154-9f79cd25-aca9-4091-8db6-392ae1b27b48.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>Test 5 - Can add up to 3 toppings<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197426187-55e964ea-afd6-4b0d-85e2-8ea3263584f6.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>Test 6 - cost must be calculated properly based on the choices (check<br>for currency format as part of this) (test case should have a few<br>permutations of choices)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197426231-2d3100ab-e285-4b8d-bc4e-842aec858f80.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>Test 7 - Total Sales (sum of costs) must be calculated properly (test<br>case should included a few icecream combinations/purchases)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197426347-b0e9db6f-13ba-4859-b148-ba78f8099333.jpg"/></td></tr>
<tr><td> <em>Caption:</em> <p>Test 8 - Total icecreams should properly increment for each purchase<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197426434-deda5f7a-2386-42a3-8de8-903699daf1d7.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>1-8testings<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Summarize each test case logic</td></tr>
<tr><td> <em>Response:</em> <div><div>Test 1: This test ensures that the container is the top option.</div><div>Test 2:<br>In this test, it ensures that the ice cream is flavored with the<br>available flavors.</div><div>Test 3: The toppings that are in stock can only be added<br>in this test.</div><div>Test 4: It ensures that no more than three scoops are<br>used.</div><div>Test 5: The ice cream toppings are limited to three.</div><div>Test 6: It makes<br>sure that formatting and cost calculations are done appropriately.</div><div>Test 7: It guarantees that<br>the total sales are correctly computed.</div><div>Test 8: After every purchase, ice creams should<br>be accurately incremented.</div></div><br></td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 4: </em> Misc </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add pull request for the assignment</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/5">https://github.com/Kotapavankumar1/IS601-005/pull/5</a> </td></tr>
<tr><td> <em>Sub-Task 2: </em> Explain any issues/difficulties or something you learned while doing this assignment</td></tr>
<tr><td> <em>Response:</em> <div>I first considered handling exceptions in the file icecream exceptions. Later, I understood<br>that it should be handled in the Ice cream Machine file.</div><div>I gained knowledge<br>about how to manage exceptions and ensure good operation.<br></div><div>I also learned about Pytest<br>and how it functions as well as how it aids in the development<br>of better programs.<br></div><br></td></tr>
<tr><td> <em>Sub-Task 3: </em> Screenshots of successful output</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197429596-13acd26b-9633-4baf-b160-0085aa0081fb.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>In this ,I ordered only scoop vanilla and got cost of 2.75<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197429638-383c7e80-db49-4144-bf74-94f5c7ad541f.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>In the above screenshot ,I tried with adding two scoops(chocolate and vanilla) and<br>got the cost of 3.25<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/197429658-fb9fecdc-851e-4a15-844b-f3b4f16870c7.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>In this screenshot, I added  three scoops(vanilla, chocolate and strawberry) with different<br>flavours and i got the cost of 4.25<br></p>
</td></tr>
</table></td></tr>
</table></td></tr>
<table><tr><td><em>Grading Link: </em><a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-mini-project-1-icecream/grade/pk639" target="_blank">Grading</a></td></tr></table>