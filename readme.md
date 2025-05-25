# 📂Project Setup
<pre> 
  Assignment-2-HTML-CSS-Based-Web-Form-Manual-Testing-Scenarios/ 
    ├── 10 positive and 5 negative test scenarios.pdf
    ├── index.html 
    ├── readme.md 
    ├── style.css
</pre>
# 🛠️ Build commands
> [!TIP]
> No Build Command needed. Open the Registration form by opening the html file(index.html).
# ✅ A brief description of functionalities
 - **Purpose** - Ensuring user friendly application form is interactive and easily understandable by the users and returns the text to check user input are taken correctly.
## Dark Mode setup
```javascript
  function changeMode(){
        // Getting elements by id value for modifying
        const body = document.getElementById("_body");
        const formcolor = document.getElementById("form");
        const text = document.getElementById("changemode");
        /*The below code toggles the style for 
        1. Background of body [white <-> black]
        2. Text color in the form [white <-> black]
        3. Text on button between [Light mode <-> dark mode]*/ 
        if (body.style.backgroundColor === "white"){
            body.style.backgroundColor = "black";
            formcolor.style.color = "white";
            text.innerText = "Light Mode";
        }
        else{
            body.style.backgroundColor = "white";
            formcolor.style.color = "black";
            text.innerText = "Dark Mode";
        }
    }
```
