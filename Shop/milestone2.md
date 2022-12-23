<table><tr><td> <em>Assignment: </em> IS601 Milestone 2 Shop Project</td></tr>
<tr><td> <em>Student: </em> Pavan Kumar Kota Ravi (pk639)</td></tr>
<tr><td> <em>Generated: </em> 12/22/2022 7:31:16 PM</td></tr>
<tr><td> <em>Grading Link: </em> <a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-milestone-2-shop-project/grade/pk639" target="_blank">Grading</a></td></tr></table>
<table><tr><td> <em>Instructions: </em> <ol><li>Checkout Milestone2 branch</li><li>Create a new markdown file called milestone2.md</li><li>git add/commit/push immediate</li><li>Fill in the below deliverables</li><li>At the end copy the markdown and paste it into milestone2.md</li><li>Add/commit/push the changes to Milestone2</li><li>PR Milestone2 to dev and verify</li><li>PR dev to prod and verify</li><li>Checkout dev locally and pull changes to get ready for Milestone 3</li><li>Submit the direct link to this new milestone2.md file from your GitHub prod branch to Canvas</li></ol><p>Note: Ensure all images appear properly on github and everywhere else. Images are only accepted from dev or prod, not local host. All website links must be from prod (you can assume/infer this by getting your dev URL and changing dev to prod).</p></td></tr></table>
<table><tr><td> <em>Deliverable 1: </em> Users with admin or shop owner will be able to add products </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshot of admin create item page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208785273-684b14fe-4692-40c0-82a7-6e9e3b0ea0df.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>Show valid data filled in<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add screenshot of populated Products table clearly showing the columns</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208785564-af2429d4-680f-4586-9472-0e180ca1fcd5.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>db screenshot of Columns: (id, name, description, category, stock, created, modified, unit_price, visibility<br>[true, false])<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Briefly describe the code flow for creating a Product</td></tr>
<tr><td> <em>Response:</em> <div><ul><li>When the form is submitted with valid data, I check the arguments to<br>see if an id is present to confirm whether it is an edit<br>or create operation. If there is no id, the server validates using the<br>validate on submit function.</li><li>Once validated, all of the information is entered into the<br>database and a message is displayed to confirm the creation.</li><li>If an error occurs,<br>a message is displayed.</li></ul></div><br></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
<tr><td> <em>Sub-Task 5: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/admin/product">https://is601-pk639-prod-2.herokuapp.com/admin/product</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 2: </em> Any user can see visible products on the Shop Page </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot of the Shop page showing 10 items without filters/sorting applied</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208812982-28787b97-aa80-406b-9a31-cc01af803017.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of 5 products<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208813032-4b762e8e-1365-422b-ba02-2723f82633b1.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshots of remaining 5 products<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot of the Shop page showing both filters and a different sorting applied (should be more than 1 sample product)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208813183-f584f91f-3855-4b45-b357-9e58dfa6c4d9.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of filter and sort applied in the page<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add a screenshot of the filter/sort logic from the code</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208789301-a3a6ccaf-e623-45e0-a3e7-4481f8508810.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>filter/sort logic code with ucid and date mentioned<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 4: </em> Briefly explain how the results are shown and how the filters are applied</td></tr>
<tr><td> <em>Response:</em> <div>• The category list dropdown is generated on page load by accumulating the<br>category types in the database.</div><div>• If any of the filters are selected, the<br>corresponding filters are appended to the fetching query.</div><div>• All products are retrieved from<br>the database, with filters applied if any have a stock greater than zero,<br>and visibility is set to true.</div><div>• If an error occurs while retrieving products,<br>a message is displayed.</div><br></td></tr>
<tr><td> <em>Sub-Task 5: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
<tr><td> <em>Sub-Task 6: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/shop?product_name=&category=&sort_by=unit_price&order=desc&limit=10">https://is601-pk639-prod-2.herokuapp.com/shop?product_name=&category=&sort_by=unit_price&order=desc&limit=10</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 3: </em> Show Admin/Shop Owner Product List (this is not the Shop page and should show visibility status) </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Screenshot of the Admin List page/results</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208790730-8e774cb5-ab5a-4a38-9e31-ea45c8f29607.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>non visible products with admin heroku dev url<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Briefly explain how the results are shown</td></tr>
<tr><td> <em>Response:</em> <div><ul><li>All product details, including non-visible items, are retrieved. In the query logic, visibility<br>is marked true if 1 and false otherwise.</li><li>The retrieved products are rendered using<br>table helper.html.</li></ul></div><br></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/admin/product/list">https://is601-pk639-prod-2.herokuapp.com/admin/product/list</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 4: </em> Admin/Shop Owner Edit button </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot showing the edit button visible to the Admin on the Shop page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208791149-4c8e2e5d-b5dc-4aa0-8848-3f7f5bc20bdf.png"/></td></tr>
<tr><td> <em>Caption:</em> <p> screenshot showing the edit button visible to the Admin on the Shop<br>page<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot showing the edit button visible to the Admin on the Product Details Page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208791355-22c17e5a-738c-4647-b537-c7378d30e67c.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing the edit button visible to the Admin on the Product Details<br>Page<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add a screenshot showing the edit button visible to the Admin on the Admin Product List Page (The admin page)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208791515-e8c0da34-4848-4422-b24a-7c896ee8505e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>a screenshot showing the edit button visible to the Admin on the Admin<br>Product List Page (The admin page)<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add a before and after screenshot of Editing a Product via the Admin Edit Product Page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208791912-bc1eec37-b099-4d0b-b3bd-e18aba21da73.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>before editing a product<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208792179-ee2dbcaa-21cb-4984-a8e2-e1dc131fcba2.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>after editing title, description, stock and also cost<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208792363-b99d6e76-8809-49d3-9ea6-e559073b126b.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>admin page after editing<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 5: </em> Briefly explain the code process/flow</td></tr>
<tr><td> <em>Response:</em> <ul><li>The edit page accepts an id as an argument and preloads the form<br>with its details.</li><li>Following the update of the values and the click of "Edit<br>Product," an update query is used to update all of the values in<br>the database.</li><li>A flashing message indicates whether the operation was successful or not.</li></ul><br></td></tr>
<tr><td> <em>Sub-Task 6: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
<tr><td> <em>Sub-Task 7: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/admin/product?id=11">https://is601-pk639-prod-2.herokuapp.com/admin/product?id=11</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 5: </em> Product Details Page </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot showing the button (clickable item) that directs the user to the Product Details Page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208807057-bc69deb9-329a-4389-b076-13c903abacfb.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing the button (clickable item) that directs the user to the Product<br>Details Page Checklist<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot showing the result of the Product Details Page</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208807156-0492b6c3-4409-4c79-a2eb-9ca77adf4a2e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot showing the result of the Product Details Page<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Briefly explain the code process/flow</td></tr>
<tr><td> <em>Response:</em> <div><ul><li>When you click a product title on the shop list page, the product<br>details page is loaded, with the corresponding id as an argument.</li><li>The id is<br>retrieved from the arguments, and all product details are retrieved from the database.</li><li>These<br>particulars are displayed in a horizontal card layout.</li></ul></div><br></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
<tr><td> <em>Sub-Task 5: </em> Add a direct link to heroku prod for this file (can be any specific item)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/admin/productDetails?id=6">https://is601-pk639-prod-2.herokuapp.com/admin/productDetails?id=6</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 6: </em> Add to Cart </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a screenshot of the success message of adding to cart</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208807349-1e56c30d-a903-4aaf-8795-b53092931814.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of the success message of adding to cart<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a screenshot of the error message of adding to cart (i.e., when not logged in)</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208797099-86e332a0-1503-4cb5-9898-a6c39597f510.png"/></td></tr>
<tr><td> <em>Caption:</em> <p> screenshot of the error message of adding to cart (i.e., when not<br>logged in)<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add a screenshot of the Cart table with data in it</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208811661-4509e180-5896-44b8-8785-70206ae0effb.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of the Cart  in UI <br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208812138-bd15bc0a-ee33-4b78-95e5-77ec8fe1fb70.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of the Cart table with data in it<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 4: </em> Tell how your cart works (1 cart per user; multiple carts per user)</td></tr>
<tr><td> <em>Response:</em> <p>The cart functions as one cart per user, to which the user can<br>add multiple products.<br><br></p><br></td></tr>
<tr><td> <em>Sub-Task 5: </em> Explain the process of add to cart</td></tr>
<tr><td> <em>Response:</em> <div><ul><li>When you add a product to the cart by clicking the "+Add" button,<br>the corresponding id and quantity are passed to the cart route</li><li>Cart populates the<br>cart table with the product id, quantity, cost, and user id.</li><li>If the item<br>is already in the cart, the quantity is update.</li></ul></div><br></td></tr>
<tr><td> <em>Sub-Task 6: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 7: </em> User will be able to see their Cart </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add screenshot of the Cart View</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208809481-9e5c3e70-5c8d-42e3-bc78-9958fbc0f033.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>cart view<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208809375-85d7756e-29fa-4746-8a9a-adc1e4091016.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>cart view with different products<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Explain how the cart is being shown from a code perspective along with the subtotal and total calculations</td></tr>
<tr><td> <em>Response:</em> <div>• All of the information stored in the cart table is retrieved and<br>displayed.</div><div>• Each item's subtotal is calculated based on the unit price and quantity<br>in the select query.</div><div>• The total is calculated by adding all of the<br>subtotals while rendering with Jinja2's namespace.</div><br></td></tr>
<tr><td> <em>Sub-Task 3: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
<tr><td> <em>Sub-Task 4: </em> Add a direct link to heroku prod for this file</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/cart">https://is601-pk639-prod-2.herokuapp.com/cart</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 8: </em> User can update cart quantity </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Show a before and after screenshot of Cart Quantity update</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208812504-fb3f38d4-1058-4632-9085-b74a04fc05d0.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of cart before quantity update of 1 beanie<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208812567-417e5919-f8b0-4499-81fe-7b238fe8f59e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of cart after quantity updating the 1 beanie to 6<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Show a before and after screenshot of setting Cart Quantity to 0</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208808775-5522a7e3-e399-482c-8b9d-8f67a867c44c.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of college bag product before of setting Cart Quantity to 0<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208808440-5e455283-bfff-43f3-bf07-89474bea84a8.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot after setting cart to 0 which makes college bag deleted<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Show how a negative quantity is handled</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208809967-57e31ba6-3479-4a2b-9452-27d1476a106a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>negative quantity will delete the product from the cart<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 4: </em> Explain the update process including how a value of 0 and negatives are handled</td></tr>
<tr><td> <em>Response:</em> <div>•When the update button is pressed, the product id is sent in the<br>post request, indicating that an update has occurred.</div><div>• The quantity is changed to<br>match the product id.</div><div>• If the quantity is greater than zero, the update<br>is skipped. If not, the associated product is removed from the card.</div><br></td></tr>
<tr><td> <em>Sub-Task 5: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 9: </em> Cart Item Removal </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Add a before and after screenshot of deleting a single item from the Cart</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208810127-87a70160-3ef1-43ff-8f04-e750ab662a8e.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>before deleting single item from the cart<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208810260-70aa7195-27a6-496c-a429-4c6300b6e48a.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>after deleting single item from the cart<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a before and after screenshot of clearing the cart</td></tr>
<tr><td><table><tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208810451-cd0e8b1e-1959-41f0-9a11-1c0152864a2f.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of before clearing the data<br></p>
</td></tr>
<tr><td><img width="768px" src="https://user-images.githubusercontent.com/113547463/208810658-3cc0fbe7-7604-405e-bf5a-b8caee5feed6.png"/></td></tr>
<tr><td> <em>Caption:</em> <p>screenshot of after clearing the data<br></p>
</td></tr>
</table></td></tr>
<tr><td> <em>Sub-Task 3: </em> Briefly explain how each delete process works</td></tr>
<tr><td> <em>Response:</em> <div>• Deleting each product follows the same logic as updating the quantity.</div><div>• When<br>the delete button is clicked, we pass a negative quantity value, which deletes<br>the corresponding product from the cart.</div><div>• On Clear all, I send action clear<br>in the post request, and when that condition is met, it deletes all<br>of that user's products from the database by matching user id.</div><br></td></tr>
<tr><td> <em>Sub-Task 4: </em> Add related pull request link(s)</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://github.com/Kotapavankumar1/IS601-005/pull/21">https://github.com/Kotapavankumar1/IS601-005/pull/21</a> </td></tr>
</table></td></tr>
<table><tr><td> <em>Deliverable 10: </em> Misc </td></tr><tr><td><em>Status: </em> <img width="100" height="20" src="http://via.placeholder.com/400x120/009955/fff?text=Complete"></td></tr>
<tr><td><table><tr><td> <em>Sub-Task 1: </em> Describe any issues and learnings throughout this milestone</td></tr>
<tr><td> <em>Response:</em> <p>I attempted to implement file upload for images while adding new products, and<br>while it worked fine locally, it did not work on Heroku.&nbsp;<div>I used a<br>different approach, adding host image URLs to render images.&nbsp;</div><div>I learned and practiced how<br>to efficiently reuse the code for similar actions such as deletion and changing<br>the quantity to 0 or less.</div><br></p><br></td></tr>
<tr><td> <em>Sub-Task 2: </em> Add a link to your herok prod project's login page</td></tr>
<tr><td> <a rel="noreferrer noopener" target="_blank" href="https://is601-pk639-prod-2.herokuapp.com/login">https://is601-pk639-prod-2.herokuapp.com/login</a> </td></tr>
</table></td></tr>
<table><tr><td><em>Grading Link: </em><a rel="noreferrer noopener" href="https://learn.ethereallab.app/homework/IS601-005-F22/is601-milestone-2-shop-project/grade/pk639" target="_blank">Grading</a></td></tr></table>