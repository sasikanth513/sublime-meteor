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


- console logging `console.log($1);`
    ```sh
    lg
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
      var self = this;
      self.dataDict = new ReactiveDict();
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

> ### toastr

- toastr error `toastr.error("$1", "Error");`.
    ```sh
    te
    ```
    
- toastr info `toastr.info("$1", "Info");`.
    ```sh
    ti
    ```
    
- toastr error `toastr.success("$1", "Success");`.
    ```sh
    ts
    ```