[[ HTML Forms Guide ]]

Form Actions and Buttons:

-> form "action" represents to where the data of the form will go (to a server maybe)

	<form action="https://www.freecatphotoapp.com/submit-cat-photo"></form>

-> the input type is specified and the "placeholder" is the pre-text in the grey in the text field. A field will be "required" and won't submit the form unless the field is filled with the info 

	<input type="text" placeholder="cat photo URL" required>

-> a checkbox/radio button will be "checked"  if the keyword checked is written in the input tag
	
	<label for="indoor">
  		<input id="indoor" type="radio" name="indoor-outdoor" checked>Indoor
	</label>

-> the button will make a button in the form field with the name text specified before the closing tag

	<button type="submit">Submit</button>

--> final code (with all the things embedded):

	<form action="https://www.freecatphotoapp.com/submit-cat-photo">
    	<input type="text" placeholder="cat photo URL" required>
    	<button type="submit">Submit</button>
  	</form>

==========================================================================

Radio Buttons:

-> Radio buttons are used for questions where you want the user to only give you "one answer" out of multiple options

-> Radio buttons are a type of "input" & Each of your radio buttons can be nested within its own "label" element

	<input id="indoor" type="radio" name="indoor-outdoor">
	<label for="indoor">Indoor</label>

--> Nested radio buttons having the same name but individual labels:

	<label for="indoor">
  		<input id="indoor" type="radio" name="indoor-outdoor">Indoor
	</label>

    
	<label for="outdoor">
  		<input id="outdoor" type="radio" name="indoor-outdoor">Outdoor
	</label>

============================================================================

Checkboxes in a form:

-> Checkboxes are used for questions where you want the user to only give you "more than one answer" out of multiple options

-> Checkboxes are a type of "input" & Each of your checkbox can also be nested within its own "label" element

--> Three checkboxes having the same name but different individual labels:

	<label for="koot">
		<input id="koot" type="checkbox" name="personality"> Koot
	</label>
    
    <label for="loving">
    	<input id="loving" type="checkbox" name="personality"> Loving
    </label>
    
    <label for="adorable">
    	<input id="adorable" type="checkbox" name="personality"> Adorable
    </label>

==========================================================================

Adding the "value" attribute:

-> The data goes to the server in the pattern "name=value"

-> If you omit the value attribute, the submitted form data uses the default value, which is "on" (e.g personality=on)

-> This is for both Radio Buttons and Checkboxes

--> Labels with the "value" attribute embedded are:
	
	Radio Button:

		<label for="indoor">
			<input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor
		</label>

	Checkbox:

		<label for="lazy">
			<input id="lazy" type="checkbox" name="personality" 
			value="lazy"> Lazy
		</label>
	