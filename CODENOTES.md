// a program state is pulling values out of variables
// these variables are stored in the scope
//Tokenizing = breaking up a string of characters into meaningful chunks, called tokens
//considering if "a" is part of another token, or an individual token is called lexing
//AST or Abstract Syntax Tree is when you take an array and you turn it into nested elements
var a = 2; //var is variable declaration, a is identifier, the = is assignment expression and the 2 is the numeric literal
//Code Generation is when you take AST and turn it into executable code
# The Cast
 1. Engine: Responsible for start to finish compilation of a Javascript program
 2. Compiler: Handles the dirty work of parsing code
 3. Scope: Looks at all the declared identifiers (Variables)
  with the program var a = 2;
  The compiler will break it down into tokens. The compiler asks the scope if
  "a" already exists. If not, the compiler asks the scope to declare a new variable
  named "a". Compiler then produces code to have Engine execute. The engine
  also asks the scope if a is accessible in that scope selection. If engine finds
  a then it will convert its value to 2
# LHS and RHS statement (right hand and left hand side)
with var a = 6; var a is the LHS and the 6; is the RHS
Left hand is about declaration and right hand is about the values

#scope
You have a function scope and a lexical scope.
function foo () {
  var b = 'b';
}

{
  var d = 'd'
  let c = 'c';
}
The var ignores the fact that its in a block, (d).  
