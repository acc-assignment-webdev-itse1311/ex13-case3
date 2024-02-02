# NP HTML5, CSS3, and JavaScript 6e Tutorial 13, Case Problem 3

## Description:
```angular2html

1.  Use your editor to open the mas_register_txt.html, mas_register_txt.js, mas_reg2_txt.html, and mas_reg2_txt.js from the html13 > case3 folder. Enter your name and the date in the comment section of each file, and save them as mas_register.html, mas_register.js, mas_reg2.html, and mas_reg2.js respectively
2.  Go to the mas_register.html file in your editor. Add a script element for the mas_register.js file. Load the file asynchronously.
3.  Take some time to study the contents of the file, taking note of the field names and IDs assigned to different form controls. Save your changes to the file.
4.  Return to the mas_register.js file in your editor. Directly below the initial comment section, insert an event listener for the window load event. Run an anonymous function in response to the event containing the following commands:

    a. Call the calcCart() function (which you will create shortly).
    b. Create an onclick event handler for the regSubmit button that runs the sessionTest() function when the button is clicked.
    c. Create onblur event handlers for the input boxes with the IDs: fnBox, lnBox, groupBox, mailBox, phoneBox, and banquetBox, running the calcCart() function in response to each event.
    d. Create an onchange event handler for the sessionBox selection list, running the calcCart() function when the selection list is changed.
    e. Create an onclick event handler for the mediaCB check box, running the calcCart() function in response.
5.  Create the sessionTest() function. The purpose of this function is to provide a validation test for the conference session selection list. Add the following commands to the function:
    a. Test whether the selected index of the sesssionBox selection list is equal to -1. If it is, the user has not selected a session package. Display the custom validation message "Select a Session Package".
    b. If the selected index is equal to -1 set the custom validation message to an empty text string.
7. Create the calcCart() function. The purpose of this function is to calculate the registration cost and to save information about the customer's choices in session storage. Add the following commands to the function:
    a. In the session storage variable confName, store the value "firstName lastName" where first- Name and lastName are the values of the firstName and lastName fields in the regForm form.
    b. Store the values of the group, email, phoneNumber, and banquetGuests fields in the session storage variables: confGroup, confMail, confPhone, and confBanquet
    c. The cost of the banquet is $55 per guest. Multiply the value of the banquetGuests field by 55 and store the result in the session storage variable confbanquetcost.
    d. Record which session the user has selected. If the selected index of the sessionBox selec-tion list is not equal to -1, store the text of the selected option in the session storage variable confsession and the value of the selected option in the confsessioncost sesson storage vari- able; otherwise store an empty text string and the value 0 respectively.
    e. The user can opt to purchase a media pack for $115 containing gifts from the conference. If the user has clicked the mediaCB check box, store the values "yes" and 115 in the confPack and confPackcost session storage variables; otherwise store the values "no" and 0.
    f. Calculate the total registration cost by storing the value session + banquet + media in the conffotal session storage variable, where session, banquet, and media are the values of the confSessionCost, confBanquetCost, and confPackCost session storage variables. (Hint: Use the parseFloat() method to add the numeric values of the data fields.)
    g. Call the writeSessionValuesO function.
7. Display the values of the session storage variables in the current web page by creating the writeSessionValuesO function, adding the following commands:
    a. Set the text content of span elements with the IDs "regName", "regGroup", "regEmail", "regPhone", "regSession", "regBanquet", and "regPack", to thevalues of the session storage variables, confName, confGroup, confMail, conf-Phone, confSession, confBanquet, and confPack.
    b. Set the text content of the span element with the ID "regTotal" to the value $total where total is the value of the confTotal session storage variable.
8.  Document your work in the file with comments and then save the file.
9.  Open the mas_reg2.html file in your editor. Add a script element for the mas_reg2.js file. Load the file asynchronously. Save your changes to the document.
10.  Open the mas_reg2.js file in your editor. Directly below the comment section, copy and paste the writeSessionValuesO function from the mas_register.js file.
11.  Add an event listener that runs the writeSessionValuesO variable when the page loads. Save your changes to the file.
12.  Open the mas_register.html file in your browser. Verify the following:
     a. Values and selected options from the registration form are automatically displayed in the page as you tab from one control element to the next.
     b. You cannot submit the form unless a conference session packet has been selected.
     c. When the form is submitted, the browser displays the content of the mas_reg2. html file with the user's choices automatically retrieved from the session storage variables and displayed at the top of the page. Note: If you are testing your code on the Edge or Internet Explorer browsers, you must load the solution files to a server. Session storage will not be activated for files loaded on your local computer.

```
