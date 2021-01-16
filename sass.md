# Learning Sass

here i m going to teach you how to use saas btw this is a chetsheet for me in case i forget anything 

**STEP 1** : Installing Live Sass Compiler 
- go to the exetensions tab 
- search for live sass compiler
- press install 

**STEP 2** : Creating SASS files
sass files have the exetension of .scss

Now go ahead and create a folder known as styles and create inside it styles.scss
As browsers dont understand scss we cconvert scss to css using the package we just installed 

**STEP 3**
in ur style.scss file write any css code like
```scss
header {
    background : lightblue:
}
```

then press f1 and search for live sass watch sass
which we will watch ur sass and convert it into scss then ur browser can read

## Using Sass 

- creating variables

```scss 
$nameofvariable : value ;
```

- nesting 
as we know header ahas a button so w can add the folownig 
```scss 
header {
    color : pink ; 
    button {
        color : blue;
        background-color : violet;
    }
}
```

- nesting pseudo element 
u can add & instead of its name
```scss
    header {
        button {
            color : pink ;
            &::after {
                content : "hello";
            }
        }
    }
```
- separatioon of code 
  
  **STEP 1** : create new file known as _header.scss

  **STEP 2** : then u write
  ```scss
  @import "nameoffile.scss"
  ```

- creating a function 
```scss 
    @mixin nameoffunctoin (parameter) {
        display : parameter ; 
    }
```

to import it write
```scss 
header {
    @include nameofunction(flex);
}
```