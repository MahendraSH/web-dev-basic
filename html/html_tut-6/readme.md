# forms and input 
### elemets and type or attributes 

* form ```<form>``` 
    * method ```method ="post" /"get " ```
    * action ```action ='url' ```
* lable ``` lable  ```
    * for 
    ``` 
        <lable for="FirstName">FirstName</lable>
    ```
    
* input ```input``` 
    * type 
        * text ```<input type="text" name="FirstName" id="FirstName" autocapitalize="on" autocomplete="on" required> ``` 
        * date 
        * time 
        * password ```<input type="password" name="password" id="password" placeholder="password" required>```
        * tel   
        * number ```<input type="number" name="number" id="number" value="1980" min="1890" max="2020" step="10" required >```
    * name 
    * id 
    * class
    * placeholder 
    * autocomplete="on" / "of" 
    * required 
    * autofocus -----only one element in the page input can have it "|"
*  select 
```<select name="color" id="color">
            <option value="#fff">white</option>
            <option value="#000">black</option>
            <option value="#f00;">red</option>
            <option value="#0f0">green</option>
            <option value="#00f" selected>blue</option>

        </select>
```
* radio
```
    <label for="pizza">pizza</label>
    <input type="radio" name="food" id="pizza" />
    </p>
    <p>
    <label for="burger">burger</label>
    <input type="radio" name="food" id="burger" />
    </p>
```
*list discritionn list 
```
<input type="text" name="coffee" id="coffee" list="coffee-list">
            <datalist id="coffee-list">
                <option value="coffee">
                <option value="latte">
                <option value="espresso">
                <option value="cortado">
                <option value="americano">
                <option value="other">
            </datalist>
        
```
* checkBox
```
<p>
        <label for="cow">cow</label>
        <input type="checkbox" name="cow" id="cow">
      </p>
      
      <p>
        <label for="dog">dog</label>
        <input type="checkbox" name="dog" id="dog">
      </p>
      <p>
        <label for="other">other</label>
        <input type="checkbox" name="other" id="other">
      </p>
```
* button submit post reset 

```

    <button type="submit">Submit</button>
    <button type="reset">Reset</button>
    <button formaction="https://httpbin.org/post" formmethod="post">post</button>
```
* textarea ```textarea```

* fieldset ```<fieldset> ```
* legend  ```<legend>```

### form examples


```

            <form action="https://httpbin.org/get" method="get">
                <fieldset>
                    <legend>Personal Info</legend>
                    <p>
                        <label for="firstName">First Name:</label>
                        <input type="text" name="firstName" id="firstName" placeholder="Jane" autocomplete="on" required
                            autofocus>
                    </p>
                    <p>
                        <label for="lastName">Last Name:</label>
                        <input type="text" name="lastName" id="lastName" placeholder="Doe" autocomplete="on" required>
                    </p>
                    <p>
                        <label for="password">Password:</label>
                        <input type="password" name="password" id="password" placeholder="your secret" required>
                    </p>
                    <p>
                        <label for="phone">Phone:</label>
                        <input type="tel" name="phone" id="phone" placeholder="5555555555"
                            pattern="[0-9]{3}[0-9]{3}[0-9]{4}" required>
                    </p>
                    <p>
                        <label for="decade">Favorite Decade:</label>
                        <input type="number" name="decade" id="decade" min="1950" max="2020" step="10" value="1980">
                    </p>
                    <p>
                        <label for="coffee">Favorite Coffee:</label>
                        <select name="coffee" id="coffee" multiple size="5">
                            <optgroup label="Coffees">
                                <option value="regular coffee">Regular Coffee</option>
                                <option value="iced coffee">Iced Coffee</option>
                            </optgroup>
                            <optgroup label="Espresso Drinks">
                                <option value="latte" selected>Latte</option>
                                <option value="cappuccino">Cappuccino</option>
                                <option value="cortado">Cortado</option>
                                <option value="americano">Americano</option>
                            </optgroup>
                            <option value="other">Other</option>
                        </select>
                    </p>
                    <!-- <p>
                    <label for="coffee">Favorite Coffee:</label>
                    <input type="text" name="coffee" id="coffee" list="coffee-list">
                    <datalist id="coffee-list">
                        <option value="coffee">
                        <option value="latte">
                        <option value="espresso">
                        <option value="cortado">
                        <option value="americano">
                        <option value="other">
                    </datalist>
                </p> -->
                </fieldset>
                <br>
                <fieldset>
                    <legend>What is your favorite food?</legend>
                    <p>
                        <input type="radio" name="food" id="tacos" value="tacos">
                        <label for="tacos">Tacos</label>
                    </p>
                    <p>
                        <input type="radio" name="food" id="pizza" value="pizza">
                        <label for="pizza">Pizza</label>
                    </p>
                    <p>
                        <input type="radio" name="food" id="other" value="other">
                        <label for="other">Other</label>
                    </p>
                </fieldset>
                <br>
                <fieldset>
                    <legend>Do you have pets?</legend>
                    <p>
                        <input type="checkbox" name="pets" id="dog" value="dog">
                        <label for="dog">Dog</label>
                    </p>
                    <p>
                        <input type="checkbox" name="pets" id="cat" value="cat">
                        <label for="cat">Cat</label>
                    </p>
                    <p>
                        <input type="checkbox" name="pets" id="fish" value="fish">
                        <label for="fish">Fish</label>
                    </p>
                    <p>
                        <input type="checkbox" name="pets" id="otherPet" value="otherPet">
                        <label for="otherPet">Other</label>
                    </p>
                </fieldset>
                <br>
                <fieldset>
                    <legend>Send Me A Note</legend>
                    <label for="message">Your Message:</label>
                    <br>
                    <textarea name="message" id="message" cols="30" rows="10"
                        placeholder="Type your message here"></textarea>
                </fieldset>
                <br>
                <button type="submit">Submit</button>
                <button type="submit" formaction="https://httpbin.org/post" formmethod="post">Post</button>
                <button type="reset">Reset</button>
            </form>

            

```


![image](./img/Web%20capture_8-4-2023_155546_127.0.0.1.jpeg)
![imgage2](./img/Web%20capture_8-4-2023_163450_127.0.0.1.jpeg)
