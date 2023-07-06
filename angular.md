<div align="center">
  <h1>Angular</h1>
</div>

<ol>
<li>
  
**Performance Optimization in angular ?**

- `Using AoT Compilation`
- `Using OnPush Change Detection Strategy`  
- `Detach Change Detection/NgZone`  
- `Using Pure Pipes`  
- `Unsubscribe from Observables`
- `Lazy Loading`  
- `Preloading Modules`  
- `Use trackBy option for For Loop`  
- `Avoid computation in template files`
- `Usage of Web Workers`  
- `Resolve Guards`
- `Service Worker`
- `Server-side rendering`
- ` Angular Command Line Interface (CLI)`  
- ` Tree-shaking`  

</li>

---

<li>
  
  **How many directives are there ?**
  
  |No.| Types |
  |---|--------|
  | 1 | Attribute | 
  | 2 | Structural | 
  | 3 | Component |
</li>
  <li>
    
  **Diagnose  analyze Memory Leaks with Chrome DevTools steps**
    
   - `open dev tools`
   - `go to memory tab`
   - `select Allocation instrumentation`
   - `press start`
    
#### 2nd way
    
   - `open dev tools`
   - `goto more tolls`
   - `select Performance Monitor`
    
  </li>
  
  <li>
    
  **Required @Input() properties and ADDING A NULL CHECK**

  ```
@Input({ required: true }) person: string;
ngOnInit() {
  if (this.person === null || this.person === undefined) {
    throw new TypeError("The input ‘Person’ is required");
  }
}
  ```  
  </li>
  <li>
   
  **make your application faster**
  - Pure Pipes TO PREVENT METHOD CALLS 
  - TRACKBY TO DECREASE THE NUMBER OF DOM MUTATIONS
  - DETACH COMPONENTS FROM THE CHANGE DETECTION
  
  </li>

  <li>
    
  **What is Tree Shaking ?**
  - `eliminate dead code or unused modules`
  - `The Angular CLI uses the Webpack bundler`
  - `reducing the download size`
  - `improving performance`
  </li>
  <li>
    
  **Web worker vs Service worker in angular**

  - `Web worker allows code in the background in separate thread without blocking main thread`
  - `Service workers are a proxy between the browser and the network.`
  - `Service workers intercepting requests, requests to a cache,enabling offline access.`
  </li>
  <li>**App Initializer**</li>
  <li>**RouteReuseStrategy***</li>
  <li>loadChildren vs children</li>
  <li>Reducer</li>
  <li>sharedService vs SharedModule</li>
  <li>Promises vs Observables</li>
  <li>Subject vs Behaviorsubject</li>
  <li>Share data in siblings</li>
  <li>Ngrx</li>
  <li>Rxjs</li>
  <li>Of vs tap</li>
  <li>ngDoCheck</li>
  <li>ViewChild</li>
<li>ChangeDetection</li>
<li>ngZone</li>

<li>

**Guards**

- There are four different types of Guards:

- CanActivate
   `Checks to see if a user can visit a route.`

- CanActivateChild
  `Checks to see if a user can visit a routes children.`

- CanDeactivate
  `Checks to see if a user can exit a route.`

- Resolve
  `Performs route data retrieval before route activation.`

- CanLoad
  `Checks to see if a user can route to a module that lazy loaded.`
`  
</li>

<li>

 **Hooks for the Component**
 constructor
This is invoked when Angular creates a component or directive by calling new on the class.

ngOnChanges
Invoked every time there is a change in one of th input properties of the component.

ngOnInit
Invoked when given component has been initialized.
This hook is only called once after the first ngOnChanges

ngDoCheck
Invoked when the change detector of the given component is invoked. It allows us to implement our own change detection algorithm for the given component.

- ngDoCheck and ngOnChanges should not be implemented together on the same component.
- ngOnDestroy
This method will be invoked just before Angular destroys the component.
Use this hook to unsubscribe observables and detach event handlers to avoid memory leaks.

**Hooks for the Component’s Children**
- `These hooks are only called for components and not directives.`
- ngAfterContentInit
Invoked after Angular performs any content projection into the component’s view (see the previous lecture on Content Projection for more info).

ngAfterContentChecked
Invoked each time the content of the given component has been checked by the change detection mechanism of Angular.

ngAfterViewInit
Invoked when the component’s view has been fully initialized.

ngAfterViewChecked
Invoked each time the view of the given component has been checked by the change detection mechanism of Angular.
</li>
</ol>  
