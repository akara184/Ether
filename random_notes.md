
# SOME RANDOM THOUGHTS ABOUT 

### Things that i should look for 
- Currying: 
  - Why bother with uncurrying function(There are some optimization ??)

### C++ and C, difference of `&` and `*`

- `&` -> "the address of"
- `*` -> "what's at"

```cpp
int x;    // Declares x as having type int.
int y;    // Declares y as having type int.
int *p;   // Declares *p as having type int, which means that p has type pointer-to-int.

p = &x;   // Uses & to get a pointer to x, and stores it in p. p now contains the value &x.
// We say that "p points to x". In other words, *p is x.
x = 10;   // Sets the value of the variable x to be 10.
y = *p;   // Gets the value 10 from x through the pointer p and stores in y. y is now 10.
*p = 42;  // x is now 42, and y is still 10.
p = &y;   // Set p to point to y instead. *p is now y.
x = *p;   // x is now 10 again.


### C++ headers and cmake
    - For gcc users:  Using g++, you can use the -I option to specify an alternate include directory:
    g++ -o main -I./source/includes main.cpp
    There is no space after the -I. For a full path (rather than a relative path), remove the . after -I.
### Notes about morphism

- Morphism:
    A morphism is a map between two objects in an abstract category.

    1. A general morphism is called a homomorphism,

    2. A morphism f:Y->X in a category is a monomorphism if, for any two morphisms u,v:Z->Y, fu=fv implies that u=v,

    3. A morphism f:Y->X in a category is an epimorphism if, for any two morphisms u,v:X->Z, uf=vf implies u=v,

    4. A bijective morphism is called an isomorphism (if there is an isomorphism between two objects, then we say they are isomorphic),

    5. A surjective morphism from an object to itself is called an endomorphism, and

    6. An isomorphism between an object and itself is called an automorphism.

- Uma categoria é formada por dois tipos de objetos: os objetos da categoria e os morfismos, que relacionam dois objetos chamados de origem e destino do morfismo. Costuma-se dizer que um morfismo é uma seta que mapeia sua origem para seu destino. Os morfismos podem ser compostos se o alvo do primeiro morfismo for igual à fonte do segundo, e a composição do morfismo tem propriedades semelhantes à composição da função (associatividade e existência de morfismos de identidade). Os morfismos geralmente são algum tipo de função, mas nem sempre é o caso. Por exemplo, um monóide pode ser visto como uma categoria com um único objeto, cujos morfismos são os elementos do monóide.

### About Monoid
- Monoid: 
    Um monoide é uma estrutura matemática simples que precisa de apenas três ingredientes:
    1. Um Conjunto: Uma coleção de coisas (números, strings, listas).Uma Operação Binária: 
    2. Uma regra para combinar duas dessas coisas e gerar uma terceira do mesmo tipo (como a soma $+$ ou a concatenação).
    3. Um Elemento Neutro: Alguém que, quando combinado com qualquer outro, não muda nada (o "zero" da operação).
    
-    /E se não tiver elemento neutro?/: 
Se você tiver um conjunto e uma operação que é associativa, mas NÃO tem um elemento neutro, o nome dessa estrutura é Semigrupo (Semigroup).

### Some thoughts about curried function and high-order function
 -  There is a process called uncurrying
 - A *higher-order* function is simply a function that takes a function as an
   argument or returns a function as a result, and /it may or may not be curried/.
 - A curried function, on the other hand, is one that /returns/ a function as its result
 - https://stackoverflow.com/questions/75724067/are-all-curried-functions-considered-higher-order-functions
 - not all curried functions are high-order
 - *Haskell definition*: Currying is the process of transforming a function that takes multiple arguments in a tuple as its argument, into a function that takes just a single argument and returns another function which accepts further arguments, one by one, that the original function would receive in the rest of that tuple. https://wiki.haskell.org/Currying  -- this wiki answer the top stackoverflow wiki, at haskell definitions its sounds like HO-FN 
 - *Uncurrying* is the dual transformation to currying, and can be seen as a form of defunctionalization. 
 - *Uncurrying* is the reverse transformation, and is most easily understood in terms of its right adjoint, the function 




 
### Data and Codata
    - https://stackoverflow.com/questions/28841260/what-is-the-difference-between-codata-and-data#29455156
    - https://gemini.google.com/share/9b805098869a

### Compilers/interpreter
#### Syntax and Semantic erros
     - https://www.learncpp.com/cpp-tutorial/syntax-and-semantic-errors/

### Unite types:
    - In the area of mathematical logic and computer science known as type theory, a unit type is a type that allows only one value (and thus can hold no information). The carrier (underlying set) associated with a unit type can be any singleton set. There is an isomorphism between any two such sets, so it is customary to talk about the unit type and ignore the details of its value. One may also regard the unit type as the type of 0-tuples, i.e. the product of no types. https://en.wikipedia.org/wiki/Unit_type

