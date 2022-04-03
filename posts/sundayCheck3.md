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
const options = {
	method: 'GET',
	headers: {
		'X-RapidAPI-Host': 'random-words5.p.rapidapi.com',
		'X-RapidAPI-Key': '0d0dad91cdmshd70ac9ca4bc57cbp14e277jsn50f8a6d27b53'
	}
};

fetch('https://random-words5.p.rapidapi.com/getRandom?wordLength=5', options)
	.then(response => response.json())
	.then(response => console.log(response))
	.catch(err => console.error(err));
```

- Problem with API key ?
- Endpoint is invalid : *Problem Worked on W3* 
__Solution__



