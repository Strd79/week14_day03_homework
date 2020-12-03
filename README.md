## Week 14, Day 3 homework - Pirates Quiz

### Requesting All Pirates

#### Question 1 Which component is responsible for requesting all the pirates?
* PirateContainer

#### Question 2 Which hook do we use to carry out the requestAll() method and when does it get triggered?
* useEffect hook and this is triggered when the PirateContainer component is loaded.

#### Question 3 The requestAll() method creates a new instance of Request() in order to gain the functionality to carry out various forms of request. Where is the Request class?
* It is located in the helpers folder within the src folder of the front-end.

#### Question 4 Which method are we using from the Request class here?
* In the requestAll() method we are using the GET method of the Request class.

#### Question 5 The PirateList component is in charge of rendering a list of pirate components. What is the pirateNodes function returning?
* An new array of pirate components with a key for each.


### Viewing a Single Pirate

#### Question 1 When we click on one of the pirates names in the pirate list, our app renders a PirateDetail component. PirateDetail is in charge of rendering the information for a single pirate. But where is it getting its props passed down from?
* From PirateContainer

#### Question 2
```
if (!pirate){
 return "Loading..."
}
```
#### What is the purpose of this code in PirateDetail?
* This is to prevent the PirateDetail component trying to load the details until there is a Pirate object available to render.

#### Question 3 In PirateDetail, to delete a pirate, we have a button with a listener "onClick" which triggers a method called "handleDelete". The handleDelete method uses a method onDelete which has been passed in as a prop from PirateContainer. Why have we passed this method down as a prop?
* Because PirateContainer is the component which handles the actual deletion and so we need to pass that function down, in order to effectively pass up the details of the pirate to be deleted by PirateContainer.


### Bonus Points Questions

#### Question 1 In PirateContainer, what does Promise.all return?
* This returns all the info stored in the DB for pirates, ships and raids, all in one go.

#### Question 2 Ideally, we want our state to live at the top of our component chain, except in one other scenario. This is when our component contains a, what?
* A form or user input fields


