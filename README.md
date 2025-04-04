:: CODE INFO ::

HTML Explanation 

  Sets up the basic structure of the web page.
  Includes metadata for character encoding and responsive design.
  Specifies the title "TempConvert Hub".
  Links to the "Roboto Mono" font from Google Fonts for a coding style.
  Contains CSS styles within the <style> tags for visual presentation.
  Contains the website's title and logo area.
  Placeholder for the website's logo (thermometer emoji).
  The main title "Temperature Converter" with a typing animation effect.
  Holds the main content of the temperature converter.
  Provides instructions to the user.
  Arranges the input and select elements for temperature conversion.
  Input field for the temperature value.
  Dropdown to choose the unit to convert from.
  Dropdown to choose the unit to convert to.
  Displays the converted temperature.
  Contains icons for social sharing and contact.
  
CSS Explanation (Short Points):

  Styles the overall appearance of the webpage.
  Sets the font to "Roboto Mono" for a coding-style look.
  Centers the content on the page using Flexbox.
  Applies a glassmorphism effect (semi-transparent, blurred background) to the main container and social icons.
  Styles the header with center alignment and padding.
  Creates the typing animation effect for the header using CSS animations (typing and blink-caret).
  Sets up a flexible grid layout for the temperature converter form.
  Styles the input field, select dropdowns, and the result display.
  Defines CSS animations (cold-blink and hot-glow) that are applied to the body background based on the temperature.


JavaScript Functions Explanation (Short Points):

  setBackgroundColor(celsius):
  Changes the body's background color based on the Celsius temperature value.
  Adds CSS classes (cold, pleasant, warm, hot, cold-animation, hot-animation) to the body to apply specific background colors and animations.
  
capitalizeFirstLetter(string):
  Takes a string as input and returns it with the first letter capitalized.
  Used to format the unit names in the output string.

checkAndConvert():
  Checks if the temperature input field has a value and if both 'fromUnit' and 'toUnit' select dropdowns have a selected value.
  If all conditions are met, it calls the convertTemperature() function to perform the conversion.
  If not, it clears the content of the resultDiv and resets the body's background color to the default.

shareOnWhatsApp():
  Gets the current URL of the webpage.
  Creates a formatted message to share, including the URL.
  Opens a new window to the WhatsApp share link with the message.

Event Listeners:
  temperatureInput.addEventListener('input', checkAndConvert);: Calls checkAndConvert() whenever the user types in the temperature input field.
  fromUnitSelect.addEventListener('change', checkAndConvert);: Calls checkAndConvert() whenever the user changes the selected unit in the 'fromUnit' dropdown.
  toUnitSelect.addEventListener('change', checkAndConvert);: Calls checkAndConvert() whenever the user changes the selected unit in the 'toUnit' dropdown.
  checkAndConvert();: This line is executed once when the script loads to handle any initial state (although the form starts empty).


Functionality Points:

  Temperature Conversion: Converts temperatures between Celsius, Fahrenheit, and Kelvin.
  Real-time Updates: Performs the conversion and updates the result automatically as the user types or selects units.
  Dynamic Background: Changes the background color of the page based on the converted temperature in Celsius.
  Typing Title: The website's title "Temperature Converter" in the header has a typing animation effect when the page loads.
  Social Sharing: Includes icons to share the website on WhatsApp and to contact via email.


Features Points:

  User-friendly interface for temperature conversion.
  Supports three temperature units: Celsius, Fahrenheit, and Kelvin.
  Real-time conversion results.
  Visually appealing dynamic background that reflects the temperature.
  Stylish coding font (Roboto Mono).
  Modern glassmorphism design effect.
  Engaging typing animation for the title.
  Fully responsive layout that works well on various devices (desktops, tablets, and mobile phones).
  Easy contact via email with a pre-filled subject line.
