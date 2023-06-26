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
</ol>  
