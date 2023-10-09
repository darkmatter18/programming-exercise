# Event Loop Order


What's the output?

```js
function main(){
    console.log('A');
    setTimeout(
        function print(){ console.log('B'); }
        ,0);
    console.log('C');
}
main();
```

<!-- A C B -->