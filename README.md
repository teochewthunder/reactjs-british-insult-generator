# ReactJS British Insult Generator

Generating the insult uses the following formula:
1. Action, eg. *Go and die*
2. Adjective, eg. *oblivious*
3. Curse, eg. *cunt*
4. Noun, eg. *buffalo*

Together, it forms *Go and die, you oblivious cunt buffalo*.

In the `render()` method, the insult is formed from lists of words stored in four different arrays, corresponding to the formula above. Then the resultant string is rendered.

The index pointers to the arrays are stored in the component's `state`. Every time there is a change to the `state`, the rendered string will change. This is handled by the `changeInsult()` method, which changes the pointers in the `state` using random number generators.

`changeInsult()` is also run upon loading the page. This is achieved using the `componentDidMount()` method.
