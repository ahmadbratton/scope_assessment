## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.
Scope is what  variables a function can access based on where the variable is in ones code.
Hoisting is the order in which java Script orginazes variables within function to read them.
compartmentalization is storing variables inside of diffrent scopes so that variables don't make changes where you don't want them too.

### Provide examples for all three, below:

#### Scope:
var global = "global scope"
function (){
    var local = "local scope"
}

#### Hoisting:
function hoist(){
    

    var top = function(){};
}

hoist();
the var top has been hoisted but not var top = function(){}; so when hoist is called top is not assinged.

#### Compartmentalization:

var money = "80000$"

(function broke(){
    var money = "18$"

})();

money is is compartmenilized inside of the function broke and won't effect other functions the use the varbable money that is in the global scope.


