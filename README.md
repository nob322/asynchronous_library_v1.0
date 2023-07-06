                                                         asynchronous_library_v1.0
Library created by me in 2023 to facilitate asynchronous requests to and from Php written by David Sanchez - nob32_2@hotmail.com


Ej:  operationSR('123','respuesta1','recibo.php','POST','todo ok form 1',0,'Fallo el asincronismo');

To use the library, you must first include it in the project using for example something like <script src="asinchronous_library_v1.0.js"></script> (it always depends on the path where you have the asynchronous_library_v1.0.js file).
The second step is to put the following parameters in a <script></script>... tag.
operationSR('123','response1','receipt.php','POST','everything ok form 1',0,' asynchronism failed');
The parameters can be understood in the following order... first the id of the form where we want to use asynchronism (where we are going to send the form to be processed), second we must enter the id of the html tag where we want to receive the responses from the server, For example, in a <p></p> tag, third, we must specify the name and path of the Php file where we are going to send the form, fourth, the method that we will use in our asynchronism, only two options: POST or GET, fifth, we must specify a message that will be accompanied in the console with a counter that will be shown in the browser console each time an asynchronous operation is performed, for example it is recommended to put something like all ok -form name or identifier- since that will add to the console a text like the following "asynchronous operation n°x", sixth... add the number from which we want that counter to start counting, 0 is recommended, seventh and last add an error message to be displayed in the console in case of that the operation failed.

It is also important to mention that if you need to apply asynchronism to more than one form on the same page, it is enough to establish a new call to the function and add the necessary arguments, for example ---> operationSR('456','response2','receipt.php','POST','everything ok form 2',0,'Asynchronism failed');
