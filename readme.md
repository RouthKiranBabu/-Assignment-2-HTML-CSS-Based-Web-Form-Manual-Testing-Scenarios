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
## Registration form Setup
```html
    <form id = "form" action="">
        <!-- Add class="wdxl-lubrifont-tc-regular"
         To look Text nicer eg: Name, Email, etc-->
        <h2 class="wdxl-lubrifont-tc-regular">Registration Form</h2>
        <!-- Wherever class="wdxl-lubrifont-tc-regular"
             is added its makes into google fonts. -->
        <label class="wdxl-lubrifont-tc-regular" for="">Name👉</label>
        <!-- 
         1. Required: To make sure user provides input(must).
         2. id is provided to take values in javascript like
            const name = document.getElementById('name').value.trim(); 
         3. type="text": meaning user providing values is taken as text.-->
        <input id = "name" type="text" required>

        <!-- br is provided to break the line or to move to next line -->
        <br><br>
        <!-- 
        1. class="wdxl-lubrifont-tc-regular": for styling the text. Using google fonts.  -->
        <label class="wdxl-lubrifont-tc-regular" for="">Email📧</label>
        <!-- 
        1. id = "email": For taking values in script like:
           const email = document.getElementById('email').value.trim();
        2. type="email": To take values from user in form of type email becouse 
           this reason it tells to provide @ or *@* format.
        3. Required: To make sure user provides input(must).-->
        <input id = "email" type="email" required>

        <!-- br is provided to break the line or to move to next line -->
        <br><br>
        <!-- 
        1. class="wdxl-lubrifont-tc-regular": for styling the text. Using google fonts.  -->
        <label class="wdxl-lubrifont-tc-regular" for="">Password🧑‍💻</label>
        <!-- 
        1. type="password": so input provided is in the form of dotted values.
        3. Required: To make sure user provides input(must).-->
        <input type="password" required>

        <!-- br is provided to break the line or to move to next line -->
        <br><br>
        <!-- 
        1. class="wdxl-lubrifont-tc-regular": for styling the text. Using google fonts.  -->
        <label class="wdxl-lubrifont-tc-regular" for="">Gender<br>
            <!-- style="padding: 0px 0px 0px 20px;"
             padding is the distance from border to the outer content.
             first 0px for top distance, next for left, then down, then
             20 px for left.
             So need to move the radio section to little bit right side -->
            <div style="padding: 0px 0px 0px 20px;">
                <!-- 
                1. name="radios": This is present in multiple elements 
                   to get all the elements.
                   let radios = document.getElementsByName('radios');
                2. value="[MALE]": For returning [MALE] value.
                   Example to understand: 
                        Step1: Use for loop to iterate all the elements by name 'radios'
                            for (let i = 0; i < radios.length; i++) {
                        Step2: Check if the element is checked
                                if (radios[i].checked) {
                                    // The below code takes the values from eg: value="[MALE]"
                        Step3: Find and get value using index.
                                    selected_gender = radios[i].value;
                                    // Once we get the check value and stored in the variable need to break the for loop
                                    break;
                                }
                            } 
                    Finally from Step3: selected_gender = radios[i].value;
                    That's how we get values/importance of providing 👉 value="[MALE]"
                    so finally (selected_gender = MALE) if element is checked.
                3. style="cursor: pointer;": Having score 1000 makes pointer to 👆 shape when hovering to below element
                4. type="radio": This type makes input to the radio. -->
                ♂️ Male<input name="radios" value="[MALE]" style="cursor: pointer;" type="radio">
                <!-- checked: for checking this radio before hand/bydefault setup -->
                ♀️ Female<input name="radios" value="[FEMALE]" style="cursor: pointer;" type="radio" checked>
            </div>
        </label>
        
        <br>
        <!-- 
        1. class="wdxl-lubrifont-tc-regular": for styling the text. Using google fonts.  -->
        <label class="wdxl-lubrifont-tc-regular" for="">Country🚩</label>
        <!-- 
        1. select: for selecting any one from the option by default value is India at beginning.
        2. id="selectedcountry": It is used to make sure script takes value by using below code
           const selectedcountry = document.getElementById("selectedcountry").value; -->
        <select name="" id="selectedcountry">
            <!-- value="INDIA": India value is stored in variable 'selectedcountry' 
             if India is selected -->
            <option value="INDIA">India</option>
            <option value="RUSSIA">Russia</option>
            <option value="AFRICA">Africa</option>
            <option value="JAPAN">Japan</option>
            <option value="CHINA">China</option>
            <option value="OTHERS">Others</option>
        </select>

        <br><br>
        <!-- 
        1. class="wdxl-lubrifont-tc-regular": for styling the text. Using google fonts.  -->
        <label class="wdxl-lubrifont-tc-regular" for="">
            <!-- 
            1. style="cursor: pointer;": For making mouse arrow to look like 👆 making user it is on the element
            2. type="checkbox": Makes into checkbox type input.-->
            <input style="cursor: pointer;" type="checkbox">Accept Terms
        </label>

        <br><br><br>
        <!-- Since div is block type element so made the text align to center
            #submit{
                text-align: center;
            } -->
        <div id="submit">
            <!-- 
            1. class="wdxl-lubrifont-tc-regular": for styling the text. Using google fonts. 
            2. type="submit": Is another type of input. Behaves as button without button tag. -->
            <input class="wdxl-lubrifont-tc-regular" type="submit">
        </div>
    </form>
```
# Result 👇
<div align = "center">
  <img src = "https://github.com/RouthKiranBabu/Assignment-2-HTML-CSS-Based-Web-Form-Manual-Testing-Scenarios/blob/main/result.gif"/>
</div>
