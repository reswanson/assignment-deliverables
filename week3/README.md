# Week-3-deliverables

## I got prop and state features working in a test project, but when I went to add those to my main project, I was Unable to figure out how to pass props when using Route.  Let me know if you have any ideas to try.   I tried these different calls to no avail:
* <Route exact path="/props-through-render" render={(props) => <PropsPage {...props} title={`Props through render`} />} />  
* <Route path='/mybooks' render={routeProps => <Books {...routeProps} booksGetter={getMyBooks}/>} />  
* <Route exact path="/props-through-render" render={(props) => <PropsPage {...props}      title={`Props through render`} />} />  
* <Route path="/greeting/:name" render={(props) => <Greeting text="Hello, " {...props} />} />  
* <Route exact path='/' render={(props) => <LoginForm {...props} doesitwork="2" userName={this.onChangeUserName.bind(this)} />} />  
* <Route path="/" render={(props) => <LoginForm  doesitwork="Hello" {...props} />} />  
* <Route path="/" doesitwork="Hello" component={Form}/>  
* <Route path="/" render={MyLoginForm} />  
* <Route path='/' render={routeProps => <LoginForm {...routeProps} doesitwork="yesitdoes"/>}  />  
* <Route path="/" render={(props) => <LoginForm doesitwork="yesitdoes"/>}/>  
 
## SO,  I am submitting TWO projects which each have different features, yes, I might get a grade hit, but I just couldn't break my <Route> linking.
## The first project/app is my original:
### React project is here: https://github.com/reswanson/my-react-project
### Heroku link is: https://rswanson-assignment1.herokuapp.com/
### This project shows these week3 deliverables:
* An additional Page that is used to display books present in the data file.  My goal of this was that you could browse the catalog without logging in
* I added an image to the /browse page including an ugly listing of books
* I include event handling using the 'changeuser' and 'changeuserback' buttons to modify the local username, (will be used to clear or default a value)
* Reading data from a json data file
* Using a key element in my data.map(), in Showbooklist.js, to prevent the missing key error
* Passing prop from parent to child  in two ways: 
** I pass the data file that is to be read, but I couldnt figure out how to change the import process to read the datafile from inside the Component class
** Also, I pass the currently logged in username to the header field, but that isn't wired up as I couldnt pass props in <Route>
 



## I have a second git project and Heroku app which meet other requirements of this weeks assignment.

### https://github.com/reswanson/week3-myreactproject
### https://week3-myreactapp.herokuapp.com/

### This project shows the following deliverables:

* Passing props with a callback so the Submit on the LoginForm will update the HEADER with the user that is logged in.  I think this shows props and state, ( parent -> child), (child to parent) and (child to child) as the username has to flow all the way back thru.
* I figured since the original requirements called for different permissions based on the USER, I should get that value soon.
* The /browse link doesnt work as I was doing my development and had stripped some of the functionality of my test-project to simplify learning the states and props.  So the second page doesnt exist in this App.

