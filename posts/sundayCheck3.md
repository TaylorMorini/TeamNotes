---
title: Sunday Check 3
description: This is check in 3
date: 2022-04-03
tags: second tag
layout: layouts/post.njk
---

## Frontend Week 3 Work
- insert front end stuffs

## Backend Week 3 Work

**Rough Draft of WordGenerate.js**

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/m4jgp7nbcviucklutlss.png)

 
**Hashing out WordGenerate.js**
```
import fetch from 'node-fetch';
import {key} from './word.js';
export {wordGenerate};

function wordGenerate()
{
fetch('https://random-words5.p.rapidapi.com/getRandom?wordLength=5', {
"method": "GET",
"headers": {
	"x-rapidapi-key": key,
	"X-RapidAPI-Host": "random-words5.p.rapidapi.com"
}

})  
.then(response =>response.json())
.then(response => {
    console.log(response);
    console.log(response.content);
})
.catch(err => {
    console.error(err);
});
}
```
**Word.js**
- This is where the API key is 
```
var config = { API_KEY : '0d0dad91cdmshd70ac9ca4bc57cbp14e277jsn50f8a6d27b53' };

let key = config.API_KEY;

export {key};
```

- Problem with API key ? -> "api key is invalid"
   - entry issue?

**What the API end points are**
- Currently: using a random word generator API
- How it is used: this is used to get random words. one of the parameters is to set the word to
   5 letter; this way there are never words that are less than/more than 5 letters long




