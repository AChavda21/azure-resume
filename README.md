# azure-resume
My own  Azure Resume

## First step

- Frontend folder contains the website.
- main.js contains visitors counter code.

```js
window.addEventListener('DOMCotentLoaded', (event) => {
    getVisitCount();
})

const functionApi = '';

const getVisitCount = () => {
    let count = 30;
    fetch(functionApi).then(response => {
        return response.json()
    }).then(response => {
        console.log("Website called function API.");
        count = response.count;
        document.getElementById("counter").innerText = count;
    }).catch(function(error){
        console.log(error);
    });
    return count;
}
```

