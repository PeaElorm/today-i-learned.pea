# Forms and Validation 
Before the data in forms are submitted to the server, there are checks done to ensure the data matche the correct format(form control). This is called Client-side validation.

A form control is an element that enable user interactions with the form: `<input>`, `<textarea>`, `<button>`, `<select>`.

## Using Forms To Get Data From Your Users
We use the `<form>` element and wrap it around other elements like `<input>`, `<textarea>` to get the data. once the user fills the form and hits the CTA button, the browser makes a request and script can respond to that request and process the data.
By default, this request is made to the page the form is being rendered. Eg. 
```
<form action="https://example.com/accounts>
...
</form>
```
A script on the `example.com` backend can handle requests to the `/accounts` and then the data is processed.
* By default form data is sent as a `GET` request. you can change it by doing `<form method="post"></form>`
  * This is because of historical or technical reasons, not necessarily because it is the optimal choice for all situations.
    **Here's why GET is the default:**
     * Historical context: When HTML and HTTP were first developed, the web was primarily a document retrieval system. GET was the fundamental operation for accessing resources.
     * Simplicity: GET requests are simpler to process and don't require special handling of request bodies.
     * Idempotence: GET requests are meant to be idempotent (can be repeated without side effects), aligning with the original vision of HTML forms as primarily for retrieving or filtering information.
   
     NB: For forms that process sensitive data, use the `POST` method. This will make it only accessible to the backend scripts that processes the request. If the data is sharable, you can use the `GET` method; that way, it can be added to your browser history as it is included in the URL. This is useful in search forms.

    `[source:](https://web.dev/learn/forms/form-element)`


    ✅Using the appropriate form control helps you build better forms
    * `<label>` elements allow us briefly state what we are expecting the user to enter into the form field. eg. input
      ```
      <label for="favBook">What is your favorite Book?<label>
      <inout type="text" id="favBook" name="favBook">
      ```
      Note that the `for` attribute in the works in labels like it the `id` works in input. The `id` connects the input and the label
    
