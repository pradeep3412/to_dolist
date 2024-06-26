todolist link https://todo-list-evamalinina.vercel.app/
# Create Todo React App easily with Material UI

To begin:
<br />
`npx create-react-app my-app`
<br />
`cd my-app`
<br />
`npm start`

Delete all default mark up.

For components create folder #components in #src folder and place there your react components.
In my project you can see: Form.jsx, FormInput.jsx, List.jsx.
You can create as many components as you want and name it how you like.

In this project Material-UI is used.
To install run:
<br />
`npm install @material-ui/core`

Material-UI was developed based on the Roboto font.
The Roboto font will not be automatically loaded into Material-UI.
*So be sure to install it.*

To install run:
<br />
`npm install fontsource-roboto`

Then import it in "index.js". To do so write in "index.js":
<br />
`import 'fontsource-roboto'`;

To use icons run:
<br />
`npm install @material-ui/icons`

Button example:
```
import  React from 'react';
import Button from "@material-ui/core/Button";

// custom styles with Material UI
const useStyles = makeStyles({
    root: {
        background: 'linear-gradient(45deg, gray 30%, black 90%)',
        border: 0,
        color: 'white',
        height: 30,
        padding: '0 10px',
        whiteSpace: 'nowrap',
        margin: '15px 0 0 20px',
    }
});


const Button = () => {
   const classes = useStyles();
    
   return (
      <Button
           type="submit"
           alt="add-note"
           className={classes.root}
       >
           Add task
       </Button>
     )
     
export  default Button;
```

Then you can see the result - button "ADD TASK" look like:

![Button example](https://github.com/EvaMalinina/todo-list-react-hooks/blob/master/src/demo/button%20git.gif)

That was easy, right :)



