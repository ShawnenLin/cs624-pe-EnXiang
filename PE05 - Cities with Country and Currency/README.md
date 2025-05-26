# INPUT
Users input string values in two of the four screens: Add City and Add Country.
Submissions can be made by the users by pressing the submit button on these two forms.

*Users can choose an item from their lists of Cities and Countries for further information.

# PROCESS
When the user types something into any of the input fields, the application detects the value change.

When the user submits their information from either the add city form or the add country form, the program checks first to see if both the fields in the form are filled. If they are, the information is added to the respective object properties (city or country) and the object is routed through the top-level routing params in order to make it available to all components. The input form gets reset to its original state and the user gets taken to the page in which their information was added (cities or countries).

*When a user clicks on an item in one of their lists (cities or nations), a navigation event occurs to bring the user to a page whose title matches the name of the city or nation the user clicked on -- yet no routes exist for this action.

# OUTPUT
The load screen sets the app to launch on the Cities page. A default message of "No saved cities!" is displayed.

Four navigation tabs at the bottom of the screen are: Cities, Add City, Countries, Add Country.

The Add City and Add Country pages each feature a form with two input fields.

The placeholders specify what should be filled into each field (city name & country name; country name & currency name, respectively).

The Countries page has the appearance of the Cities page when loaded.

A message displays by default: "No saved countries!"

When a user types into an input text field, the user will see the text input replace the placeholder. On a failed user submit action, an alert will appear warning the user to verify both form fields contain valid information. On a successful submission of the form, the user will be forwarded to a page where the user's new inputted information will fill.

Return to either the add city or add country pages will bring a new blank form to input additional user entries.

When multiple instances of a form submission have been received, the latest information fills in at the bottom of the list being displayed. *If either list item on the page for the cities or the page for the countries is clicked, an error will occur since the route handling has not been defined.