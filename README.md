# Country-guide-app
It starts by selecting the search button element and the country input field element from the HTML document using their respective IDs.

An event listener is added to the search button using the addEventListener method. It listens for a click event and executes the callback function when the button is clicked.

Inside the callback function, the value entered in the country input field is assigned to the countryName variable.

The finalURL variable is created by concatenating the base URL (https://restcountries.com/v3.1/name/) with the countryName value and some additional query parameters (?fullText=true).

The fetch function is used to make a GET request to the finalURL. The response is converted to JSON format using the response.json() method.

The data from the response is logged to the console for testing purposes. It includes information such as capital, flag image URL, common name, continent, currencies, languages, population, and maps.

The result element (not shown in the code) is populated with HTML markup using template literals. The retrieved data is inserted dynamically into the HTML markup.

Finally, there are some commented out error handling code blocks that can be used to display error messages if the fetch request fails or if the input field is empty or contains an invalid country name.

Live Demo:https://countrys-guide-app.netlify.app/
