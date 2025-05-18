# Semantic HTML
This the use of HTML markup for their purpose rather for their appearance. It involves using HTML elements that clearly define their purpose and content. eg. <nav>for navigation contents</nav> instead of using a div.

### Why should we care?
1. It improves accessibilty, SEO and code redability. 
2. It also helps screen readers interpret the contents of a page.
3. By using semantically correct elements, we create applications that are meaninful to both humans and machines.
4. It helps search engines understand the structure and purpose of the content of your site.

### Some common HTML elements and their use cases
* `<header></header>` this is for the top section of your page. you want your title, logo and navigations link here.
* `<nav></nav>` This for your navigation. By using it, both your users and search engine know that this section of your site is specifically for navigation.

  ```html
  //without semantics
  <div class="nav">
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact us</a>
  </div>

  // with semantics
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact us</a></li>
    </ul>
  </nav>
  ```

  * `<main></main>` for the main section of your web page
    
    ```html
    // without semantics
    <div class="main-content">
      <p>This is the main content</p>
    </div>

     // with semantics
    <main class="main-content">
      <p>This is the main content</p>
    </main>
    ```

    ... you get the drill

    *  `<article></article>` for standalone piece of content like a blog post or a product review. Note that the content within this element should make sense on it own. It can include images, heading, paragraphs.
   
    *  `<aside></aside>` this is part of the main content but usually contains supplementary information, a side nav, extra info.
    *  `<section></section>` to group closely related items
    *  `<footer></footer>` this for information like copyright, contact details and your socials
    *  `<details>` and `<summary>` this is for collapsible contents
        ![image](https://github.com/user-attachments/assets/ecb39aa9-ea10-473b-9700-1a2670635d88)
    * `<figure>` and `<figcaption>` see this is adding a content and then having to caption it or give a brief info about it
        ![image](https://github.com/user-attachments/assets/554f7ee5-de0f-45db-8d83-5f9ff3204233)
    * `<mark>` use the mark tag to highlight texts; An important info or a search result
      ![image](https://github.com/user-attachments/assets/e440af1a-5eaa-4eef-aec4-c36232a7e00d)
    * `<time>` use the time tag to allow search engines know you are talking about a specific time. they identify it easier.
    * ![image](https://github.com/user-attachments/assets/ca0ff9cb-0632-476d-9e61-ce2c3eeac0e9)
    * `<progress>` used to markup a progress bar.
    * ![image](https://github.com/user-attachments/assets/44839a48-fe40-4dce-9453-6cb455c79694)
   
    ### Summary
    With sematics, its not about asthetics its about writing HTML with meaningful and purposeful elements. this helps the user, enables search engines and assistive devices perform better!






