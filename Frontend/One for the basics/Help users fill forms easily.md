### Making the most of autofill
Filling forms can be time-consuming and statistics say 3 out of 4 people abadon form filling based on a number of factors. For example, have to repeated re-enter your address and email on every site you visit can become annoying, especially when you quickly just want to shop and go.
![image](https://github.com/user-attachments/assets/b374f84f-e915-437b-97c6-b55822d1e09c)

Drum rolls... autofill to the rescue! You can enter your address once and then the browser will start to suggest it to the user evrytime they come accross a similar form field.

### How does autofill work in browsers?
  * Browsers use `heuristics` or rules of thumb to identify similar fields. They do these by checking what the values for `name`, `value`, `id` attributes are. They also check if there is an `autocomplete` atrribute present on the form control. Based on these, they can offer the correct autofill options

  * ### So do developers help browsers autofill?
  *   * By using the appropriate formm attributes as mentioned earlier.
  *   * specifically adding the autofill attribute to the field. Note that you can turn it off if the data is sensitive. like so:
        ``` html
            <input name="sscode" id="sscode" autocomplete="off">
        ```
        <img width="538" alt="image" src="https://github.com/user-attachments/assets/79e2ccc5-a692-406b-b0c4-bc2735ce5bca" />
        Now the browser can recommend all the names i have filled in a properly atrributes name filled before.

        Note: This helps for convinience but its not always safe. You need to be more security conscious about sensitive form fields

