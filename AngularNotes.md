## Angular
### Command
1. ng serve --open - to open angular application
2. npm install -g @angular/cli -> Installs Angular CLI globally
3. ng new <project name> -> Creates a new Angular application
4. ng serve --open -> Builds and runs the application on lite-server and launches a browser

5. ng generate <name> -> Creates class, component, directive, interface, module, pipe and service
6. ng build -> 	Builds the application

## template statement
<button type="button" (click)="message subscribed successfully">Subscribe</button>
{{message}}
<button type="button" (click)='Subscribe()'>Subscribe</button>

## Structural directive
<h3>ngif Demo</h3>
<div *ngIf='!submited'>
    <h2>Login form</h2>
    <form >
        <input type="text" placeholder="enterName" #name>
        <input type="password" placeholder="enter Password" #pass>
        <button type="button" (click)='handleSubmit(name.value,pass.value)'>Login</button>
    </form>
</div>
<div *ngIf='submited'>
    <h3 *ngIf='!isvalid'></h3>
</div>
