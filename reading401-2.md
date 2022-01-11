# Readings: Node Ecosystem, TDD, CI/CD


1. Describe (in plain English) what Array.map() does

- Returns a new array with results from a used function.

```Javascript
const array1 = [1, 4, 9, 16];
// pass a function to map
const map1 = array1.map(x => x * 2);
```

2.Describe (in plain English) what Array.reduce() does

-Reduce does not change the original array, it returns a single value based on the executed reducer function for the array. Is a total result will be one value. The reducer will only return one value.

```Javascript
const array1 = [1, 2, 3, 4];
const reducer = (previousValue, currentValue) => previousValue + currentValue;
```

3.Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
With normal Promise .then() syntax

```Javascript
const map1 = new Map()
superagent.get('https://swapi.dev/api/people/')
  .then(data => {

    data.body.results.forEach((value, key) => {
      let newData = data.set(value.name, value.url)
    })
    console.log(newData)
  })

  .catch(err => console.error(err))

```

Again with async / await syntax

```Javascript

async function cityData(cityName) {
  superagent.get(await `https://geocode.xyz/${cityName}?json=1`)
  .then(data => {
    console.log(data.body.standard.city,data.body.longt,data.body.latt)
})

 .catch(err => console.error(err))
}

cityData('seattle');
cityData('chicago');
cityData('new york');
cityData('Los Angeles');

```

4.Explain promises as though you were mentoring a Code 301 level student

- A promise is an object that represents the completion or failure of an async function and the result. The promise will complete or fail based on if it ever recieves what it is expecting. Yo can specify the time of the wait.

5.Are all callback functions considered to be Asynchronous? Why or Why Not?

- No, every asynchronous function takes a function argument, but not every function that does so is asynchronous.