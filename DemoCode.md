      function Header({ title }) {
        console.log(title); // "React"
        return <h1>{title}</h1>;
      }

      // An object property with dot notation
      function Header(props) {
        return <h1>{props.title}</h1>;
      }
      
      // A template literal
      function Header({ title }) {
        return <h1>{`Cool ${title}`}</h1>;
      }
      
      // The returned value of a function
      function createTitle(title) {
        if (title) {
          return title;
        } else {
          return 'Default title';
        }
      }
       
      function Header({ title }) {
        return <h1>{createTitle(title)}</h1>;
      }

      // ternary operators
      function Header({ title }) {
        return <h1>{title ? title : 'Default Title'}</h1>;
      }