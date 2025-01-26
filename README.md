ACEPRO

	Author:
			Palaniappan S (coeusepalani)
	 		Profile URL:https://github.com/coeuspalani


	Overview:
		This Project Consist of two pages "FormHub" and  "GetHere", designed to recieve the inputs from the user via form and displaying the preview of data throungh data persistence using localstorage with Responsive UI design.
		 
			1.FormHub:
            		This Page is an User-friendly form with a perfect responsive design where users can input their details and upload an image. This is sent to localStorage (User Side ) and to the Server(Client Side)

			2.GetHere:
          			This Page retrieves the Saved data from localstorage and displays in printable format.


Features:

	1.FormHUb:

              Form-Field:
                        1.UserName
                        2.Email ID
                        3.Department
                        4.Project Link
                        5.Project Description
                        6.Profile Image        
              Validation:
                        1.Username allows only letters, numbers, and underscores.
                        2.Email, URL, and required fields are validated using HTML5 constraints.
                        3.Profile image size is restricted to 2MB.      
              Data Storage:
                        1.User-Side:Form data and Image(in Base64 format) is stored in JSON format in localStorage
                        2.Client-Side:Data is Stored in a remote Server (via API fetch) using SheetDB  
              Image-Preview:
                        1.Displays the Name of the Selected Image File and Validatesn size before uploading.
	2.GetHere:

              Display:
                        1.Details and Image is Displayed in a styled card Layout.
              Print-Friendly:
                          1.Provided printing options for ease of user.
                          2.Styled the Print Layout using "@media print".
                          3.Automatically Re-directs to the main Page After Printing.
              Responsive Design:
                          1.Adjusts Layout according to the  screen size for more readability.


How It Works:

    1.FormHub:
                1.User fills out the form and uploads an image.
                2.Form data is validated and saved in localStorage as JSON.
                3.Image is converted to a Base64 string and stored in localStorage.
                4.Data is sent to the remote server using the SheetDB API.
                5.On successful submission, the user is redirected to GetHere.
    2.GetHere:
                1.Retrieves user data (JSON and image) from localStorage.
                2.Displays user details and profile image.
                3.Includes a print button for easy printing.
                4.After printing, redirects the user back to FormHub.


SetUp and Usage:

      1.Prerequisites:
                1.A modern web browser that supports localStorage.
      2. View The Project:
                1.Project URL: https://coeuspalani.github.io/formhub/
      3.Instruction:
                1.Fill out the form on FormHub.
                2.Upload a profile image (less than 2MB).
                3.Submit the form to save data locally and send it to the server.
                4.On submission, you'll be redirected to GetHere.
                5.View your submitted data and print the page if needed.
								
Technologies Used:

                1.HTML5: Markup structure.
                2.CSS3: Styling and responsive design.
                3.JavaScript:
                      Form validation.
                      Local storage handling.
                      Fetch API for server communication.
                4.SheetDB API: For remote data storage.
File-Structure:

                project-folder/
                    |-- formhub.html
                    |-- gethere.html
                    |-- images/
                    |   |-- filebg.jpeg
                    |-- icons/
                    |   |-- favicon-96x96.png
                    |   |-- favicon.svg
                    |   |-- favicon.ico
                    |   |-- apple-touch-icon.png
                    |-- site.webmanifest  
Notes:

                1.Ensure you have an active internet connection for the Google Fonts and SheetDB API.
                2.To use the SheetDB API, replace the placeholder https://sheetdb.io/api/v1/3wdpcayk7gept and the Bearer token with your own.
                3.Clear localStorage manually if switching users or testing multiple cases.
Licence:

          			This project is open-source and free to use for learning purposes.


                          

