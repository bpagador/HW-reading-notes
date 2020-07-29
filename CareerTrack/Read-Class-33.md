#### MVVM Introduction
- model: holds data and has nothing to do with the logic
- viewmodel: connector between model and view
- view: hold formatted data and delegates everything to the model 

#### MVVM
- model: real state content OR data access layer (which is data-centric...but I thought no logic in model?)
- view: structure, layout, and appearance of what the user sees on the screen; user interaction
- viewmodel: abstraction of the view exposing public properties and commands
    - unlike--in the MVP model--the presenter (which has reference to the view), the viewmodel does not 