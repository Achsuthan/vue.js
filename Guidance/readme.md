This file is contain about the vuejs directives

1. if u want to access the values from vuejs object have to use {{ YOUR_VARIABLE_IN_VUE.JS }}

2. Capture the values form text field when user typing it use v-on:input = "YOUR_METHOD_NAME_WITHOUT_BRACKET"

3. One use the value first time later if its changed u don't need to updated it to HTML use v-once

4. If u want to use the hreft value form VUE.JS use v-bind:href="YOUR_VARIABLE_NAME"

5. v-html is used to render the text to html v-html="VARIABLE_NAME"

6. v-on:click is used to button click event v-on:click="YOUR_FUNCTION_NAME"

7. v-on:mousemove is used to do the action on move mouse v-on:mousemove="YOUR_METHOD_NAME"

7. want to pass the values through mouse evnet with event object v-on:click="YOUR_METHOUD_NAME(YOUR_PARAMETER, $event)"

8. v-on:mousemove.stop is used to stop the mousemove event v-on:mousemove.stop=""

9. v-on:keyup is used to key up event when the key release the function will get trigger v-on:keyup="YOUR_FUNCTION_NAME"

10. If we want to have a specific key press event v-on:keyup.space.enter => function will triger when user press space and enter key v-on:keyup.space.enter = "YOUR_FUNCTION"

11. Bind the text input value to vue.js object v-model="YOUR_VARIABLE_NAME"

12. watch: {} is used to check the value change handler, assume that u have a variable name called counter in vue.js code if u want to triger a function when the counter changed,
        watch: {
            counter: function(value){
                var val = value 
                console.log("this will print the count value ". val.counter)
            }
        }

13. v-on can used by @     v-bind can be used with :
    v-on:click => @click
    v-bind:href => :href

14. Adding a class to div v-bind:class="{YOUR_CLASS_NAME: TRUE/FALSE}", it will append with the external css 

15. Another way to set the class to div v-bind:class="YOUR_CLASS_NAME", if we want to have multiple class v-bind:class="[YOURCLASS_NAME,{CLASSNAME: TRUE/FALSE}]"

16. computed is used, when there any value changed, if u have a calculator, if something should happen when there is a small change in this case we can use the computed

        computed:{
            valueChange: function(){
                return {
                    backgroundColor: red
                }
            }
        }

        call valueChange this function where ever u want if the value got changed 


17. v-if is used to check a condition in vue.js  