# Welcome to URL SHORT-NER!

## About
Hi! This project is created for shortening URLs generated in sorted systems. This projects handles the task for redirecting from a short url to original URL
> The project is created with Node JS v18.17.1 (npm v9.6.7)
```mermaid
graph LR
A[Link Clicked from mail] -- 1. calls URL-shortner --> B(url-shortner) 
B --> D[2. Find the link original URL from hash] --> Z[2.1 : Check in DB]
Z -- return original URL--> B
B --> C[3. Updates the number of click] --> Y[3.1 : update click in DB]
B -- 4. Redirects to original URL --> A
```
## How to Run
|command  | pourpose |
|--|--|
|npm start  | runs with nodemon |
|node index.js|runs with node |


#### Author
- Prakhar Verma