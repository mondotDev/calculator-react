# calculator-react
## Set Up
 - ```npx create-react-app calculator-react```
 - ```cd calculator-react```
 - ```npm start```
 - Clean up public and src folders:

        | /public       | /src      |
        |---------------|-----------|
        | favicon.ico   | App.js    |
        | index.html    | index.css |
        | manifest.json | index.js  |
        | robots.txt    |           |

- in the src file add component folders/files ```mkdir components && cd components/ && mkdir Button ButtonBox Screen Wrapper && cd Button/ && touch Button.js Button.css && cd../ButtonBox/ && touch ButtonBox.js ButtonBox.css && cd../Screen/ && touch Screen.js Screen.css && cd ../Wrapper/ && touch Wrapper.js Wrapper.css```
- in Wrapper.js add:

    ```
    import "./Wrapper.css";

    const Wrapper = ({ children}) => {
        return <div className="wrapper">{children}</div>
    };

    export default Wrapper;
    ```
- in Wrapper.css add:
    ```
    .wrapper {
        width: 340px;
        height: 540px;
        padding: 10px;
        border-radius: 10px;
        background-color: #485461;
        background-image: linear-gradient(315 deg, #485461 0%, #28313b 74%);
    }
    ```