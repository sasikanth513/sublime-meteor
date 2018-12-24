# Sublime Snippets

Folders.

  - general
  - meteorjs
  - toastr

> ### general

- image thumbnail placeholder `https://randomuser.me/api/portraits/thumb/men/${1}.jpg` add number between 1 -10.
    ```sh
    ruser
    ```


- console logging: default color `console.log($1);`
    ```sh
    lg
    ```

- console logging: blue color `console.log($1);`
    ```sh
    lgb
    ```

- console logging: green color `console.log($1);`
    ```sh
    lgg
    ```

- console logging: red color `console.log($1);`
    ```sh
    lgr
    ```

> ### meteorjs

- to throw error in meteor `throw new Meteor.Error(404,"${1}");`.
    ```sh
    throw
    ```

- template hooks in js file.
    ```sh
    tpd
    ```
    
    snippet

    ```
    Template.$1.onCreated( () => {
      const t = this;
      t.dataDict = new ReactiveDict();
    });
    
    Template.$1.helpers({
    
    });
    
    Template.$1.onRendered( () => {
    
    })
    
    Template.$1.events({
    
    });
    
    Template.$1.onDestroyed( () => {
    
    });
    ```

- to `get` dataDict(reactive-dict from above snippet) value inside template helpers.
    ```sh
    tpg
    ```

    snippet

    ```
    const t = Template.instance();
    const ${1} = t.dataDict.get('${1}');
    ```

- to `set` dataDict(reactive-dict from above snippet) value inside template helpers.
    ```sh
    tpg
    ```

    snippet

    ```
    const t = Template.instance();
    t.dataDict.set('${1}', ${1});
    ```
- Template instance inside helpers.
    ```sh
    ti
    ```

    snippet

    ```
    const t = Template.instance();
    ```
    

> ### react

- component skelton.
    ```sh
    cmp
    ```
    
    snippet

    ```
    import React from 'react';

    export default class $1 extends React.Component {
      render() {
        return (
          
        );
      }
    }
    ```

> ### toastr

- toastr error `toastr.error("$1");`.
    ```sh
    te
    ```

- toastr warning `toastr.warning("$1");`.
    ```sh
    tw
    ```
    
- toastr info `toastr.info("$1");`.
    ```sh
    ti
    ```
    
- toastr error `toastr.success("$1");`.
    ```sh
    ts
    ```