<table><tr><td> <em>Assignment: </em> IS601 Milestone 3 Shop Project</td></tr>
<tr><td> <em>Student: </em> Pavan Kumar Kota Ravi (pk639)</td></tr>
<tr><td> <em>Generated: </em> 12/22/2022 11:46:01 PM</td></tr>
<tr><td> <em>Grading Link: </em> <a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-milestone-3-shop-project/grade/pk639" target="_blank">Grading</a></td></tr></table>
<table><tr><td> <em>Instructions: </em> <ol><li>Checkout Milestone3 branch</li><li>Create a new markdown file called milestone3.md</li><li>git add/commit/push immediate</li><li>Fill in the below deliverables</li><li>At the end copy the markdown and paste it into milestone3.md</li><li>Add/commit/push the changes to Milestone3</li><li>PR Milestone3 to dev and verify</li><li>PR dev to prod and verify</li><li>Checkout dev locally and pull changes to get ready for Milestone 4</li><li>Submit the direct link to this new milestone3.md file from your GitHub prod branch to Canvas</li></ol><p>Note: Ensure all images appear properly on GitHub and everywhere else. Images are only accepted from dev or prod, not localhost. All website links must be from prod (you can assume/infer this by getting your dev URL and changing dev to prod).</p></td></tr></table>
<table><tr><td> <em>Deliverable 1: </em> Orders will be able to be recorded </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot of the Orders table with valid data in it</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209252756-afc0b38d-229d-4ec9-bb39-25ef824c2612.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>DB screenshot of orders<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot of OrderItems table with validate data in it</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209252932-56adfd1f-59f8-4c46-82e9-b2a6c1215f95.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>DB screenshot of orderItems<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add a screenshot of the purchase form UI from Heroku</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209253134-f7ba720b-4923-447c-9af2-b911b513d8aa.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of the purchase form UI from Heroku<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add a screenshot showing the items pending purchase from Heroku</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209253303-90dbb7c7-48b2-43e4-88b0-37b48e84a0d1.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing the items pending purchase total purchase price and link back to<br>cart<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209260913-bedb4c58-cc76-45f7-a53f-0f15c9722088.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing % price change to the user<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 5: </em> Add a screenshot showing the Order Process validations from the code</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209253779-6be51900-efb0-4268-8d34-8634c13a456d.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>showing the Order Process validations from the code<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209254045-b5e2b0e6-6315-48fb-9036-d25319e608af.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Verify paid amount vs cart amount<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 6: </em> Add a screenshot showing the Order Process validations from the UI (Heroku)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209261265-10e98c3d-a51c-416b-92ce-6ac29ba303f9.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing the price difference message<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209261507-d096e152-1b38-4b9c-89be-7aae56ceb6fc.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>not enough stock left<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209261681-c7ff7e1b-0e11-4d46-b423-d65838e88942.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>the amount entered does not match with amount entered<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 7: </em> Briefly describe the code flow/process of the purchase process</td></tr>
<tr><td> <em>Response:</em> <div>• We have a checkout button after adding products to the cart.</div><div>•When you<br>click checkout, you're taken to the checkout page, where the same cart details<br>are retrieved from the cart table and displayed as pending items to be<br>purchased. Below it, a shipping address form will be populated.</div><div>• When entering details<br>and clicking on place order, each item quantity is checked to see if<br>it is in stock. Then, if the product's cart cost matches the product<br>cost in the database.</div><div>• To validate, the amount paid is compared to the<br>cart server value.</div><div>• If the above validations are met, the shipping information is<br>inserted into the orders table and the cart information is inserted into the<br>orderitems table; otherwise, the user is redirected to the</div><br></td></tr>
<tr><td> <em>Sub-Task 8: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/24">https://github.com/Kotapavankumar1/IS601-005/pull/24</a> </td></tr>
<tr><td> <em>Sub-Task 9: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/checkout">https://is601-pk639-prod-2.herokuapp.com/checkout</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 2: </em> Order Confirmation Page </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot showing the order details from the purchase form and the related items that were purchased with a thank you message</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209267360-9f8e8ac3-2931-4f6f-bf77-cb21a92d3951.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>successful purchase<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Briefly explain how this information is retrieved and displayed from a code logic perspective</td></tr>
<tr><td> <em>Response:</em> <div><ul><li>The cart details that are fetched for validation during the purchase are also<br>passed to render on the order summary page.</li><li>• After the order was confirmed<br>and the data was inserted into the orders table, the details were saved<br>in an array and passed to the oder summary function to render.</li></ul></div><br></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/24">https://github.com/Kotapavankumar1/IS601-005/pull/24</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/purchase">https://is601-pk639-prod-2.herokuapp.com/purchase</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 3: </em> User will be able to see their Purchase History </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot showing purchase history for a user</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209267474-7287af8b-60ba-4507-8611-b9fea8ae9a3c.png"/></td></tr>
<tr><td> <em>Caption:</em> <p> screenshot showing purchase history for a user<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot showing full details of a purchase (Order Details Page)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209270619-d93b2b9f-b1b6-438f-b8a5-0b11b4cdc5e4.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing full details of a purchase (Order Details Page)(similar to Order Confirmation<br>Page except no “Thank you” message)<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209271014-7d03749f-93d8-4647-bc6c-dbef1ab46afb.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>order details<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Briefly explain the logic for showing the purchase list and click/displaying the Order Details</td></tr>
<tr><td> <em>Response:</em> <div>The order details saved on the orders table for that user id are<br>fetched and displayed with a view button.</div><div>• When you click the view button,<br>the order id is passed to the order details page, and all the<br>details shown in the order summary page are fetched by joining the products<br>and order items tables for product details and the orders table for shipping<br>details.</div><br></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/24">https://github.com/Kotapavankumar1/IS601-005/pull/24</a> </td></tr>
<tr><td> <em>Sub-Task 5: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/orders">https://is601-pk639-prod-2.herokuapp.com/orders</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 4: </em> Store Owner Purchase History </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot showing purchase history from multiple users</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209267934-89a7b068-6c0a-4af3-9c32-38d55099edde.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing purchase history from multiple users<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot showing full details of a purchase (Order Details Page)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209267661-e3690771-613f-4fc2-9c2d-424384aa263e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing full details of a purchase (Order Details Page)<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Briefly explain the logic for showing the purchase list and click/displaying the Order Details (mostly how it differs from the user's purchase history feature)</td></tr>
<tr><td> <em>Response:</em> <p>It is similar to the user&#39;s purchase history feature, with the exception that<br>the user id filter is not applied when retrieving the orders list, so<br>the result includes orders from all users.<br></p><br></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/24">https://github.com/Kotapavankumar1/IS601-005/pull/24</a> </td></tr>
<tr><td> <em>Sub-Task 5: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/admin/orders">https://is601-pk639-prod-2.herokuapp.com/admin/orders</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 5: </em> Misc </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshot of the Cart page showing the button to place an order</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/209268212-b1b7b7cd-0add-48aa-a2f6-d7e59ebb5b8a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Cart page showing the button to place an order Preview<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Describe any issues and learnings throughout this milestone</td></tr>
<tr><td> <em>Response:</em> <div>By referring to the sample SHOP project provided in class, I learned what<br>all should be included in server-side validations for a secure purchase. I had<br>problems retrieving the order details by clicking the view button. It was resolved<br>by running a static query and debugging it in the database.</div><div>Please keep in<br>mind that where I used the same pull request, there are separate commits<br>for each feature. I forgot to merge the pull request after each feature<br>was completed, resulting in a pull request with multiple commits.</div><br></td></tr>
</table></td></tr>
<table><tr><td><em>Grading Link: </em><a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-milestone-3-shop-project/grade/pk639" target="_blank">Grading</a></td></tr></table>