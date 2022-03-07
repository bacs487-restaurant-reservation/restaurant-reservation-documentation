# React Routing Issues
- To solve this issue, I created another simple react app on my machine to test this out
# What We Did (Mainpage.js)
- Here is the structure for how to implement the links
- create a ul tag
- then create an li tag and within this tag is where you would put your code.
- here is an example of what it should look like
 -<li><button onClick={() =>(navigate("/zipcode"))} > Guest </button></li>
 - within this code we are just saying:
   - create a button
   - on click, we want to naviage to our url/zipcode
   - the button that the user will see is called Guest
 - This would be in the specific component where you want this button to be displayed
 - this button is displayed in our mainpage component


 # App.js
 - In our app.js file is where the app is essentially running from and where we are calling all of our other componenets
 - This is where we woulc import everything that we need to import from react
 - ex: import browserrouter, routes, router, along with importing all of our components
 - When we do this we first need to create a router tag, within the router tag create a routes tag and within the routes tag create a route tag
 - I'm not sure exactly what the router and routes tags do but the route is the key part
 - in the route tag you would end up having something that looks like this: <Route path="/" element={<MainPage />}/>
 - if you were to move to another page you would just put the name of that page after the /
 - Overall this is how the navigation is working


# Index.js
- the Index.js file was also giving us some issues so I figured out what we needed
- inorder for all of this to work we needed to have this code in our index.js file
- ReactDOM.render(  <React.StrictMode>    <App /> </React.StrictMode>,   document.getElementById('root')  );
- I'm also not sure what this does but when I threw this in there it worked
  
