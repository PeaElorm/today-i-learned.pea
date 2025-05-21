A scalable Framework thanks to the scaling-friendly nature of PHP

`HTTP Kernel` is a central component responsible for processing HTTP requests and generating responses.
run `php artisan serve` to view it in your local environment

Note: 
* concatenation in php is done with . instead of + in js.    
* backticks are for running shell commands here not string literals
* here, we use -> to access propertise instead of the .

## Routing in Laravel
Routing is the process of directing the user request which takes the form of urls into some specific action that can return a rsponse.
* Render the page when a specific url matches.

  The Route takes a url and a funtion as a parameter; the `url` for the specific page and the `function` what should happen shen the user navigates to that route.
<img width="425" alt="image" src="https://github.com/user-attachments/assets/ee6f8bb3-b319-4795-b366-719566ed40ef" />

figCaption: An example of static and dynamic routes

you can also redirect by using the `redirect()`
``` php
Route:: get('/hallo', function(){
    return redirect('/hello');
});
```
📝 To check all the routes in your application, run `php artisan route:list` 
